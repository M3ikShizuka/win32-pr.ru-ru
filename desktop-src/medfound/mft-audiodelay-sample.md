---
description: '\_Пример АУДИОДЕЛАЙ MFT'
ms.assetid: 08f119f9-cacd-4000-96b6-60c8c0055e9c
title: Пример MFT_AudioDelay
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 39d382ce7d1c5e9475bef85f11ef9754345e123b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460850"
---
# <a name="mft_audiodelay-sample"></a>\_Пример АУДИОДЕЛАЙ MFT

Показывает, как реализовать звуковой эффекты в виде Media Foundation преобразования (MFT). Задержка аудио MFT принимает звук PCM в качестве входных данных, применяет результат задержки (echo) и выводит измененные аудиоданные.

## <a name="apis-demonstrated"></a>Продемонстрированные API

В этом образце демонстрируются следующие интерфейсы Microsoft Media Foundation:

-   [**имфтрансформ**](/windows/desktop/api/mftransform/nn-mftransform-imftransform)

## <a name="usage"></a>Использование

В \_ образце MFT аудиоделай создается библиотека DLL, которая является сервером COM для MFT. Перед использованием MFT необходимо зарегистрировать библиотеку DLL. С помощью средства Топоедит можно создать топологию, включающую в себя временную запись MFT. Дополнительные сведения о Топоедит см. в разделе [топоедит](topoedit.md). Можно также изменить [образец плайбаккфкс](/previous-versions//bb970336(v=vs.85)) для использования MFT. Вам потребуется изменить функцию Аддбранчтопартиалтопологи в проигрывателе Player. cpp. Измените следующую строку с:

``` syntax
else if (majorType == MFMediaType_Audio)
{
    hr = CreateAudioBranch(pTopology, pSourceNode, GUID_NULL);
}
```

В:

``` syntax
else if (majorType == MFMediaType_Audio)
{
    hr = CreateAudioBranch(pTopology, pSourceNode, CLSID_DelayMFT);
}
```

Значение CLSID \_ делаймфт объявляется в файле заголовка аудиоделайууидс. h в \_ папке образца MFT аудиоделай.

## <a name="requirements"></a>Требования



| Продукт                                                        | Version   |
|----------------------------------------------------------------|-----------|
| [Windows SDK](https://msdn.microsoft.com/windowsvista/bb980924.aspx) | Windows 7 |



 

## <a name="downloading-the-sample"></a>Загрузка образца

этот пример доступен в [репозитории github для классических примеров Windows](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/multimedia/mediafoundation/mft_audiodelay).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Примеры пакетов SDK Media Foundation](media-foundation-sdk-samples.md)
</dt> <dt>

[Преобразования Media Foundation](media-foundation-transforms.md)
</dt> <dt>

[\_Пример использования градаций серого в MFT](mft-grayscale-sample.md)
</dt> <dt>

[Запись пользовательского MFT](writing-a-custom-mft.md)
</dt> </dl>

 

 
