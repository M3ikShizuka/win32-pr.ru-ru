---
title: Поддержка поздних привязок
description: Если установлена поддержка позднего связывания, каждый вызов функции должен пройти через интерфейс ADSI IDispatch, прежде чем перенаправлять его в соответствующее расширение.
ms.assetid: fbdc6234-9381-4d64-bf02-05e393b3e0bd
ms.tgt_platform: multiple
keywords:
- расширения ADSI, поддержка поздних привязок
- adsi adsi, пример кода Visual Basic, поддержка позднего связывания
- Привязка AD, поддержка позднего связывания
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f0e4dd1de0000d9edbe3e73cbc47b81d094d48c2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126970414"
---
# <a name="late-binding-support"></a>Поддержка поздних привязок

Если установлена поддержка позднего связывания, каждый вызов функции должен пройти через интерфейс ADSI [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) , прежде чем перенаправлять его в соответствующее расширение.

Рассмотрим следующий пример кода.


```C++
Set x = GetObject("LDAP://CN=JeffSmith, OU=Sales, 
                   DC=Fabrikam,DC=COM")
x.SetPassword("newPassword")
 
 
x.MyNewMethod( "\\srv\public")
x.MyProperty = "Hello World"
 
x.OtherMethod()
x.OtherProperty = 4362
 
Debug.Print x.LastName
```



Нет явных вызовов метода **QueryInterface** для получения расширений. Расширения должны перенаправлять свои вызовы [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) в интерфейс ADSI **IDispatch** . ADSI принимает решение и разрешает любые возникающие конфликты, а затем перенаправляет обратно в соответствующее расширение с помощью интерфейса с именем [**иадсекстенсион**](/windows/desktop/api/Iads/nn-iads-iadsextension). Таким образом, любое расширение, которое поддерживает позднее связывание, должно реализовывать **иадсекстенсион**.

 

 