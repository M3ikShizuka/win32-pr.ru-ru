---
title: Олицетворение и асинхронные вызовы
description: Олицетворение и асинхронные вызовы
ms.assetid: 7eaa0a66-7a80-4831-b0b6-b8eff4abd036
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0854946b619f7580173ffcbc97c9af3f2540361b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053176"
---
# <a name="impersonation-and-asynchronous-calls"></a>Олицетворение и асинхронные вызовы

Серверу не удается выполнить олицетворение клиента после вызова сервера [**исинчронизе:: Signal**](/windows/win32/api/objidlbase/nf-objidlbase-isynchronize-signal) , даже если \_ метод Begin еще не завершен. Например, предположим, что клиент вызывает метод Begin \_ , сервер немедленно обрабатывает вызов, а сервер вызывает **сигнал** , чтобы показать, что обработка завершена. Даже если работа остается в \_ методе Begin, сервер не может олицетворять клиента после завершения вызова **сигнала** .

Если сервер олицетворяет клиента перед вызовом [**сигнала**](/windows/win32/api/objidlbase/nf-objidlbase-isynchronize-signal), маркер олицетворения не будет удален из потока, пока сервер не вызовет [**Исерверсекурити:: RevertToSelf**](/windows/win32/api/objidlbase/nf-objidlbase-iserversecurity-reverttoself) или пока не выполнит вызов сервера, в зависимости от того \_ , что происходит первым.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Делегирование и олицетворение](delegation-and-impersonation.md)
</dt> <dt>

[Выполнение асинхронного вызова](making-an-asynchronous-call.md)
</dt> </dl>

 

 