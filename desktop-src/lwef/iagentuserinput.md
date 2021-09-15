---
title: иажентусеринпут
description: иажентусеринпут
ms.assetid: 59ce7337-6031-4449-8b29-fd0c6737c3e8
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7b37d195d6b5d1294c071a1b73d1da95548cb7a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570639"
---
# <a name="iagentuserinput"></a>иажентусеринпут

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

Когда сервер уведомляет входной-активный клиент с [**иажентнотифисинк:: Command**](iagentnotifysink--command.md), он возвращает сведения через объект [**иажентусеринпут**](/windows/desktop/lwef/iagentuserinput) . **Иажентусеринпут** определяет интерфейс, позволяющий приложениям запрашивать эти значения.

**Методы в порядке таблицы Vtable**



| Методы Иажентусеринпут                                         | Описание                                                                                                                              |
|-----------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| [**GetCount**](iagentuserinput--getcount.md)                   | Возвращает количество вариантов команд, возвращаемых в [**командном**](command-event.md) событии.                                         |
| [**жетитемид**](iagentuserinput--getitemid.md)                 | Возвращает идентификатор для определенной альтернативной [**команды**](command-event.md) .                                                              |
| [**жетитемконфиденце**](iagentuserinput--getitemconfidence.md) | Возвращает значение свойства [**достоверности**](confidence-property.md) для определенной альтернативной [**команды**](command-event.md) . |
| [**жетитемтекст**](iagentuserinput--getitemtext.md)             | Возвращает значение текста [**голоса**](voice-property.md) для определенной альтернативной [**команды**](command-event.md) .                   |
| [**жеталлитемдата**](iagentuserinput--getallitemdata.md)       | Возвращает данные для всех альтернативных [**команд**](command-event.md) .                                                                  |



 

 

 