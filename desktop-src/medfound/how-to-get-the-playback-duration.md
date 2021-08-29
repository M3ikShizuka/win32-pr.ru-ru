---
description: В этом разделе описывается, как получить продолжительность воспроизведения файла мультимедиа с помощью Мфплай.
ms.assetid: b1ea4f21-55d1-47b0-b6d3-8951dce79f7c
title: Как получить длительность воспроизведения
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7c715ae82c63006ef8ad375fa9624cbd65ee5516be2d3e3379e5ca58a2fb5166
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119958345"
---
# <a name="how-to-get-the-playback-duration"></a>Как получить длительность воспроизведения

\[Мфплай доступен для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. \]

В этом разделе описывается, как получить продолжительность воспроизведения файла мультимедиа с помощью Мфплай.

**Получение времени воспроизведения**

1.  Вызовите [**имфпмедиаплайер:: креатемедиаитемфромурл**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaplayer-createmediaitemfromurl) или [**Имфпмедиаплайер:: креатемедиаитемфромобжект**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaplayer-createmediaitemfromobject) , чтобы создать элемент мультимедиа для файла.
2.  Вызовите [**имфпмедиаитем:: Duration**](/windows/desktop/api/mfplay/nf-mfplay-imfpmediaitem-getduration). Укажите **МФП \_ поситионтипе \_ 100 НС** для первого параметра. Длительность возвращается в виде **пропвариант** , содержащего **большое \_ целочисленное** значение. Длительность задается в единицах 100-наносекундных.

В следующем примере показан шаг 2.


```C++
#include <propvarutil.h>

HRESULT GetPlaybackDuration(IMFPMediaItem *pItem, ULONGLONG *phnsDuration)
{
    PROPVARIANT var;

    HRESULT hr = pItem->GetDuration(MFP_POSITIONTYPE_100NS, &var);

    if (SUCCEEDED(hr))
    {
        hr = PropVariantToUInt64(var, phnsDuration);
        PropVariantClear(&var);
    }

    return hr;
}
```



## <a name="requirements"></a>Requirements (Требования)

для мфплай требуется Windows 7.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование Мфплай для воспроизведения звука и видео](using-mfplay-for-audio-video-playback.md)
</dt> </dl>

 

 



