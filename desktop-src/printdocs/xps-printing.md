---
description: Предоставляет интерфейс диспетчера очереди печати. Приложения могут использовать этот API для отправки XPS-документов на принтер.
ms.assetid: df06ddcb-e573-461c-99a3-8f108fe2c143
title: API печати XPS
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 30c53322a8ae6a03c3ac4bb71fc680f719999546
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570519"
---
# <a name="xps-print-api"></a>API печати XPS

\[API печати XPS не поддерживается и может быть изменен или недоступен в будущем. Вместо этого клиентские приложения должны использовать [API пакета печати документов](./tailored-app-printing-api.md) .\]

Предоставляет интерфейс диспетчера очереди печати. Приложения могут использовать этот API для отправки XPS-документов на принтер.

В этом разделе содержатся сведения о следующих разделах.

<dl>

[Сведения об API печати XPS](about-xps-print-api.md)  
[Использование API печати XPS](using-the-xps-print-api.md)  
[Справочник по API печати XPS](xpsprint-interfaces.md)  
</dl>

собственные Windows приложения, которые создают документы xps, например, с помощью [api документа xps](/previous-versions/windows/desktop/dd316976(v=vs.85)), могут использовать api печати xps для отправки содержимого xps-документа на принтер.

на следующей схеме показана связь api печати XPS с другими api-интерфейсами печати, которые может использовать собственное Windows приложение.

![Схема, показывающая связь API печати XPS с другими интерфейсами API печати, которые может использовать собственное приложение Windows](images/print-apis-xps.png)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**AddJob**](addjob.md)
</dt> <dt>

[API диспетчера очереди печати](print-spooler-api.md)
</dt> <dt>

[API билетов на печать](print-ticket-api.md)
</dt> <dt>

[API печати GDI](gdi-printing.md)
</dt> </dl>

 

 
