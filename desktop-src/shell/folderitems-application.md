---
description: Содержит объект приложения коллекции элементов папки.
ms.assetid: 2cd4243e-a5a6-4de4-b310-f74558ac0fbe
title: Свойство Фолдеритемс. Application (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- FolderItems.Application
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: 7f073b81106923f889ca5209c0aa492f4c4bbd60
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579582"
---
# <a name="folderitemsapplication-property"></a>Фолдеритемс. Application, свойство

Содержит объект **приложения** коллекции элементов папки.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
objApplication = FolderItems.Application
```



## <a name="property-value"></a>Значение свойства

Ссылка на объект приложения.

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



 

 




