---
description: Настройка источника мультимедиа
ms.assetid: 1378bbe6-be94-4be1-b428-5ec58dabd1fa
title: Настройка источника мультимедиа
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 809d215cf282dba1e65c21316fafda47684a2151
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257952"
---
# <a name="configuring-a-media-source"></a>Настройка источника мультимедиа

При использовании [сопоставителя источников](source-resolver.md) для создания источника мультимедиа можно указать хранилище свойств, которое содержит свойства конфигурации. Эти свойства будут использоваться для инициализации источника мультимедиа. Набор поддерживаемых свойств зависит от реализации источника мультимедиа. Не каждый источник мультимедиа определяет свойства конфигурации.

В следующей таблице перечислены свойства конфигурации для источников мультимедиа, предоставляемых в Media Foundation. Сторонние источники мультимедиа могут определять собственные пользовательские свойства.




| Источник мультимедиа | Свойства | 
|--------------|------------|
| Источник сети | См. раздел <a href="network-source-features.md">функции сетевого источника</a>. | 
| Источник носителя ASF | <ul><li><a href="mfpkey-asfmediasource-approxseek-property.md"><strong>MFPKEY_ASFMediaSource_ApproxSeek</strong></a></li><li><a href="mfpkey-asfmediasource-iterativeseekifnoindex.md">MFPKEY_ASFMediaSource_IterativeSeekIfNoIndex</a></li><li><a href="mfpkey-asfmediasource-iterativeseek-max-count.md">MFPKEY_ASFMediaSource_IterativeSeek_Max_Count</a></li><li><a href="mfpkey-asfmediasource-iterativeseek-tolerance-in-millisecond.md">MFPKEY_ASFMediaSource_IterativeSeek_Tolerance_In_MilliSecond</a></li></ul> | 




 

Чтобы настроить источник, выполните следующие действия.

1.  Вызовите **пскреатемеморипропертисторе** , чтобы создать новое хранилище свойств. Эта функция возвращает указатель **ипропертисторе** .
2.  Вызовите метод **ипропертисторе:: SetValue** , чтобы задать одно или несколько свойств конфигурации.
3.  Вызовите одну из функций создания сопоставителя исходного кода, например [**имфсаурцересолвер:: креатеобжектфромурл**](/windows/desktop/api/mfidl/nf-mfidl-imfsourceresolver-createobjectfromurl), и передайте указатель **Ипропертисторе** в параметр *ппропс* .


```C++
// Creates a media source from a URL.

HRESULT CreateMediaSource(
    PCWSTR pszURL, 
    IPropertyStore *pConfig,    // Optional, can be NULL
    IMFMediaSource **ppSource
    )
{
    IMFSourceResolver* pSourceResolver = NULL;
    IUnknown* pSource = NULL;

    // Create the source resolver.
    HRESULT hr = MFCreateSourceResolver(&pSourceResolver);

    // Use the source resolver to create the media source.
    if (SUCCEEDED(hr))
    {
        MF_OBJECT_TYPE ObjectType;

        DbgLog(L"CreateObjectFromURL");

        hr = pSourceResolver->CreateObjectFromURL(
            pszURL,                     
            MF_RESOLUTION_MEDIASOURCE,  // Create a media source.
            pConfig,                    // Configuration properties.
            &ObjectType,                // Receives the object type. 
            &pSource            
            );

        DbgLog(L"CreateObjectFromURL - FINISHED");

    }

    if (SUCCEEDED(hr))
    {
        hr = pSource->QueryInterface(IID_PPV_ARGS(ppSource));
    }

    SafeRelease(&pSourceResolver);
    SafeRelease(&pSource);
    return hr;
}
```



Сопоставитель источников передает указатель **ипропертисторе** непосредственно обработчику схемы или обработчику байтового потока, который создает источник. Сопоставитель источника не пытается проверить свойства.

Как правило, эти свойства используются для дополнительных параметров. Если не указать хранилище свойств, источник мультимедиа по-прежнему должен работать правильно с параметрами по умолчанию.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сопоставитель источников](source-resolver.md)
</dt> </dl>

 

 



