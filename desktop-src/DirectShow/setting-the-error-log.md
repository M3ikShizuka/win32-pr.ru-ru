---
description: Настройка журнала ошибок
ms.assetid: 2e3124e3-32d0-4eb6-9c1d-91b625018ac4
title: Настройка журнала ошибок
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ac96fb90570408ca41be06656f7cf1704e9f48dc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053841"
---
# <a name="setting-the-error-log"></a>Настройка журнала ошибок

\[Этот API не поддерживается и может быть изменен или недоступен в будущем.\]

После реализации класса ведения журнала ошибок создайте новый экземпляр класса. затем присвойте [DirectShow службам редактирования](directshow-editing-services.md) указатель на него, вызвав метод [**иамсетеррорлог::p ut \_ ErrorLog**](iamseterrorlog-put-errorlog.md) на временной шкале. Запросите временную шкалу для интерфейса **иамсетеррорлог** . Чтобы убедиться, что все ошибки зарегистрированы, следует вызвать этот метод перед загрузкой, сохранением или визуализацией временной шкалы.


```C++
IAMSetErrorLog  *pSetLog = NULL;
IAMErrorLog     *pLog = new CErrReporter();

pTL->QueryInterface(IID_IAMSetErrorLog, (void **)&pSetLog);
pSetLog->put_ErrorLog(pLog);
pSetLog->Release();
```



Ведение журнала ошибок не влияет на возвращаемые значения, которые вы получаете при вызове методов в приложении. Регистрация ошибок дополняет, но не заменяет стандартные методы обработки ошибок. Чтобы создать надежное приложение, всегда проверяйте значения HRESULT.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Регистрация ошибок](logging-errors.md)
</dt> </dl>

 

 



