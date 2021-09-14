---
title: Windows Типы данных журнала событий (Виневт. h)
description: Windows В журнале событий определены следующие типы данных
ms.assetid: 1aad25fe-7503-4ef8-a40a-63457bd9a007
keywords:
- EVT_HANDLE
- PEVT_HANDLE
- EVT_OBJECT_ARRAY_PROPERTY_HANDLE
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 71a93794d8cc3a254fe182c439698324dccdfc20
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241525"
---
# <a name="windows-event-log-data-types"></a>Windows Типы данных журнала событий

Windows В журнале событий определены следующие типы данных:


```C++
typedef HANDLE EVT_HANDLE;
typedef HANDLE* PEVT_HANDLE;
typedef HANDLE EVT_OBJECT_ARRAY_PROPERTY_HANDLE;
```



<dl> <dt>

**\_обработчик evt**
</dt> <dd>

обработчик для Windows объекта журнала событий.

</dd> <dt>

**ПЕВТ, \_ обработчик**
</dt> <dd>

указатель на маркер объекта журнала событий Windows.

</dd> <dt>

**\_ \_ \_ маркер свойства массива объектов \_ evt**
</dt> <dd>

маркер массива Windows объектов журнала событий.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                      |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Виневт. h</dt> </dl> |



 

 





