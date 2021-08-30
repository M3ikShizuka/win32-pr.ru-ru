---
description: В этом разделе описывается, как воспроизвести сегмент файла мультимедиа в Мфплай, установив время начала и окончания воспроизведения.
ms.assetid: cd761a4a-42ad-4994-b1b8-0946d29c3d8b
title: Воспроизведение клипа файла
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3fe8773e2658d77b6c603e121d6498a8fb5235eec16d71726049d2d59ec1169f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120061534"
---
# <a name="how-to-play-a-file-clip"></a>Воспроизведение клипа файла

\[Мфплай доступен для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. \]

В этом разделе описывается, как воспроизвести сегмент файла мультимедиа в Мфплай, установив время начала и окончания воспроизведения.

**Воспроизведение клипа файла**

1.  Вызовите [**имфпмедиаплайер:: креатемедиаитемфромурл**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaplayer-createmediaitemfromurl) или [**Имфпмедиаплайер:: креатемедиаитемфромобжект**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaplayer-createmediaitemfromobject) , чтобы создать элемент мультимедиа для файла.
2.  При необходимости получите общую длительность файла, как описано в разделе [как получить длительность воспроизведения](how-to-get-the-playback-duration.md).
3.  Вызовите [**имфпмедиаитем:: сетстартстоппоситион**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaitem-setstartstopposition) , чтобы задать время начала и окончания. Время окончания не должно превышать длительность файла.
4.  Вызовите [**имфпмедиаплайер:: сетмедиаитем**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaplayer-setmediaitem) , чтобы запустить воспроизведение.

В следующем примере используется блокирующая версия [**креатемедиаитемфромурл**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaplayer-createmediaitemfromurl). Если используется Неблокирующая версия, код, который появляется после **креатемедиаитемфромурл** , должен быть помещен в обработчик для события **МФП \_ \_ типа \_ MEDIAITEM \_ Created** . Дополнительные сведения о событиях в Мфплай см. в разделе [получение событий от проигрывателя](getting-started-with-mfplay.md).

Чтобы получить длительность файла, в этом примере вызывается `GetPlaybackDuration` функция, показанная в разделе [как получить длительность воспроизведения](how-to-get-the-playback-duration.md).


```C++
HRESULT PlayMediaClip(
    IMFPMediaPlayer *pPlayer,
    PCWSTR pszURL,
    LONGLONG    hnsStart,
    LONGLONG    hnsEnd
    )
{
    IMFPMediaItem *pItem = NULL;
    PROPVARIANT varStart, varEnd;

    ULONGLONG hnsDuration = 0;

    HRESULT hr = pPlayer->CreateMediaItemFromURL(pszURL, TRUE, 0, &pItem);
    if (FAILED(hr))
    {
        goto done;
    }

    hr = GetPlaybackDuration(pItem, &hnsDuration);
    if (FAILED(hr))
    {
        goto done;
    }

    if ((ULONGLONG)hnsEnd > hnsDuration)
    {
        hnsEnd = hnsDuration;
    }

    hr = InitPropVariantFromInt64(hnsStart, &varStart);
    if (FAILED(hr))
    {
        goto done;
    }

    hr = InitPropVariantFromInt64(hnsEnd, &varEnd);
    if (FAILED(hr))
    {
        goto done;
    }

    hr = pItem->SetStartStopPosition(
        &MFP_POSITIONTYPE_100NS,
        &varStart,
        &MFP_POSITIONTYPE_100NS,
        &varEnd
        );
    if (FAILED(hr))
    {
        goto done;
    }

    hr = pPlayer->SetMediaItem(pItem);

done:
    SafeRelease(&pItem);
    return hr;
}
```



## <a name="requirements"></a>Requirements (Требования)

для мфплай требуется Windows 7.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование Мфплай для воспроизведения звука и видео](using-mfplay-for-audio-video-playback.md)
</dt> </dl>

 

 



