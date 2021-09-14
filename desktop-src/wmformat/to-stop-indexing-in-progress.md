---
title: Завершение индексирования
description: Завершение индексирования
ms.assetid: 76c641fa-ea00-4035-bc30-a92059da584a
keywords:
- Windows Пакет SDK для формата мультимедиа, идет остановка индексирования
- Расширенный системный формат (ASF), остановка индексирования
- ASF (Расширенный системный формат), остановка индексирования
- индексы, остановка индексирования
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9ea40cbf020182250e0fb982af5b5f84327d5d9a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247240"
---
# <a name="to-stop-indexing-in-progress"></a>Завершение индексирования

После начала индексирования с помощью вызова [**ивминдексер:: startIndex**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmindexer-startindexing)индексатор обычно будет продолжать работу до индексирования файла. Можно остановить операции индексирования, вызвав метод [**ивминдексер:: Cancel**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmindexer-cancel) . После отмены индексирования можно снова вызвать **startIndex** , но индексатор будет начинаться с начала файла, а не возобновляться с момента отмены.

Поскольку **startIndex** является асинхронным вызовом, обычно требуется вызвать метод **Cancel** из другого потока или обработчика событий в приложении. как правило, **Cancel** вызывается из процедуры события, связанной с элементом управления "кнопка" Windows приложения.

При отмене индексирования индексатор передает сообщение о состоянии ВМТ \_ Closed, как будто файл был правильно проиндексирован.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Интерфейс Ивминдексер**](/previous-versions/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmindexer)
</dt> <dt>

[**Работа с индексами**](working-with-indexes.md)
</dt> </dl>

 

 




