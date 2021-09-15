---
description: Показывает, как написать декодер для Microsoft Media Foundation.
ms.assetid: 941e5400-e679-41f4-9830-3548dc6037aa
title: Пример декодера
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3dd7586534876cfa7f530e675b0342a92bf46b8a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269184"
---
# <a name="decoder-sample"></a>Пример декодера

Показывает, как написать декодер для Microsoft Media Foundation.

В этом примере реализуется макет видеодекодера MPEG-1, который отображает код времени для каждого кадра видео. На самом деле он не расшифровывает битовый поток MPEG-1. На следующем рисунке показан вывод видео из декодера.

![снимок экрана видеокадра из декодера](images/decodersample.png)

> [!Note]  
> до Windows SDK для Windows 7 этот пример был включен как часть [примера MPEG1Source](mpeg1source-sample.md).

 

## <a name="apis-demonstrated"></a>Продемонстрированные API

В этом образце демонстрируются следующие интерфейсы Media Foundation:

-   [**имфтрансформ**](/windows/desktop/api/mftransform/nn-mftransform-imftransform)

## <a name="requirements"></a>Требования



| Продукт                                                        | Version   |
|----------------------------------------------------------------|-----------|
| [Windows SDK](https://msdn.microsoft.com/windowsvista/bb980924.aspx) | Windows 7 |



 

## <a name="downloading-the-sample"></a>Загрузка образца

этот пример доступен в [репозитории github для классических примеров Windows](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/multimedia/mediafoundation/Decoder).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Примеры пакетов SDK Media Foundation](media-foundation-sdk-samples.md)
</dt> <dt>

[Преобразования Media Foundation](media-foundation-transforms.md)
</dt> <dt>

[Запись пользовательского MFT](writing-a-custom-mft.md)
</dt> </dl>

 

 



