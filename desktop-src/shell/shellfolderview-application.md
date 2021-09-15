---
description: Шеллфолдервиев. Application свойство — содержит объект приложения объекта.
ms.assetid: 305766b1-a19f-4743-a9e3-6837b3f8ffe0
title: Свойство Шеллфолдервиев. Application (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ShellFolderView.Application
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: 95ef542f91235b3b068e1b1b54768b4dd453d9b3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460320"
---
# <a name="shellfolderviewapplication-property"></a>Шеллфолдервиев. Application, свойство

Содержит объект приложения объекта.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
objApplication = ShellFolderView.Application
```



## <a name="property-value"></a>Значение свойства

Переменная типа [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) , которая получает объект приложения.

## <a name="remarks"></a>Remarks

Свойство **Application** возвращает объект автоматизации, поддерживаемый приложением, которое содержит элемент управления WebBrowser, если этот объект доступен. В противном случае это свойство возвращает объект автоматизации элемента управления WebBrowser.

это свойство можно использовать с командами **Set** и **CreateObject** или с помощью команды **getobject** для создания экземпляра Windows приложения Internet Explorer и управления им.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                           |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                           |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 4,71 или более поздняя)</dt> </dl> |



 

 
