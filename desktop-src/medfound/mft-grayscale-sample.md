---
description: Демонстрирует, как реализовать видео-эффекты в виде Media Foundation преобразования (MFT).
ms.assetid: ad7d20bc-5eab-4390-a48b-5ea8e97ead7d
title: Пример MFT_Grayscale
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ff29705476869b25aeb42157ebe4878131397988cc56eccc842fcb81134fb8db
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119102174"
---
# <a name="mft_grayscale-sample"></a>\_Пример использования градаций серого в MFT

Демонстрирует, как реализовать видео-эффекты в виде Media Foundation преобразования (MFT). Файловая таблица в градациях серого преобразует видео YUV в градации серого, устанавливая значения чрома в видео как нейтральные. Файл MFT принимает несжатое видео в форматах UYVY, YUY2 или NV12.

## <a name="apis-demonstrated"></a>Продемонстрированные API

В этом образце демонстрируются следующие интерфейсы Microsoft Media Foundation:

-   [**имфтрансформ**](/windows/desktop/api/mftransform/nn-mftransform-imftransform)

## <a name="usage"></a>Использование

\_Пример для MFT градации серого строит библиотеку DLL, которая является сервером COM для MFT. Перед использованием MFT необходимо зарегистрировать библиотеку DLL.

Чтобы просмотреть таблицу MFT в оттенках серого, запустите [Пример плайбаккфкс](/previous-versions//bb970336(v=vs.85)). Кроме того, с помощью средства Топоедит можно создать топологию, включающую основную таблицу файлов в градациях серого. Дополнительные сведения о Топоедит см. в разделе [топоедит](topoedit.md).

## <a name="requirements"></a>Требования



| Продукт                                                        | Version   |
|----------------------------------------------------------------|-----------|
| [Windows SDK](https://msdn.microsoft.com/windowsvista/bb980924.aspx) | Windows 7 |



 

## <a name="downloading-the-sample"></a>Загрузка образца

этот пример доступен в [репозитории github для классических примеров Windows](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/multimedia/mediafoundation/mft_grayscale).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Видео о YUV](about-yuv-video.md)
</dt> <dt>

[Примеры пакетов SDK Media Foundation](media-foundation-sdk-samples.md)
</dt> <dt>

[Преобразования Media Foundation](media-foundation-transforms.md)
</dt> <dt>

[\_Пример АУДИОДЕЛАЙ MFT](mft-audiodelay-sample.md)
</dt> <dt>

[Запись пользовательского MFT](writing-a-custom-mft.md)
</dt> </dl>

 

 
