---
description: Атрибуты потока байтов
ms.assetid: d57a57e9-87e4-4f7f-943a-63fd2ad1d1a6
title: Атрибуты потока байтов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bccc6b6a73d58b3b5817f6c5654a4968c3f4677c0dca9ad4d184e93ee82d8206
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119959374"
---
# <a name="byte-stream-attributes"></a>Атрибуты потока байтов

Следующие атрибуты применяются к некоторым потокам байтов. Чтобы узнать, поддерживает ли байтовый поток атрибуты, запросите объект потока байтов для интерфейса [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) .



| attribute                                                                                  | Описание                                                       |
|--------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| [**\_ \_ тип содержимого MF \_ BYTESTREAM**](mf-bytestream-content-type-attribute.md)              | Указывает тип MIME потока байтов.                         |
| [**\_Длительность BYTESTREAM \_ MF**](mf-bytestream-duration-attribute.md)                       | Задает длительность потока байтов в единицах 100-наносекундных. |
| [\_ \_ \_ URI файла ИФО BYTESTREAM \_](mf-bytestream-ifo-file-uri.md)                           | Указывает URL-адрес связанного файла ИФО.                      |
| [**MF \_ BYTESTREAM \_ \_ время последнего изменения \_**](mf-bytestream-last-modified-time-attribute.md) | Указывает, когда байтовый поток был изменен в последний раз.                   |
| [**\_ \_ имя источника MF \_ BYTESTREAM**](mf-bytestream-origin-name-attribute.md)                | Задает исходный URL-адрес для потока байтов.                     |



 

Следующие атрибуты применяются к обработчикам потока байтов.



| attribute                                                                                    | Описание                                                                                                |
|----------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| [MF \_ битестреамхандлер \_ принимает \_ общий доступ к \_ записи](mf-bytestreamhandler-accepts-share-write.md) | Указывает, может ли обработчик потока байтов использовать поток байтов, Открытый для записи другим потоком. |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**имфбитестреам**](/windows/desktop/api/mfobjects/nn-mfobjects-imfbytestream)
</dt> <dt>

[Атрибуты Media Foundation](media-foundation-attributes.md)
</dt> </dl>

 

 



