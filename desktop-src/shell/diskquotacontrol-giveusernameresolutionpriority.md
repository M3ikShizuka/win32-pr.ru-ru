---
description: Помещает указанный объект пользователя в строке для разрешения имен.
ms.assetid: 4c75f966-2e7d-4415-b1db-c98f8bdd4ce3
title: Дисккуотаконтрол. Гивеусернамересолутионприорити, метод (Дсккуота. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DiskQuotaControl.GiveUserNameResolutionPriority
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: eb5dc2939ea0fbc2c8037dc22c5b690e93a5727ecad6b2249e99e4c337340710
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119943104"
---
# <a name="diskquotacontrolgiveusernameresolutionpriority-method"></a>Дисккуотаконтрол. Гивеусернамересолутионприорити, метод

Помещает указанный объект пользователя в строке для разрешения имен.

## <a name="syntax"></a>Синтаксис


```JScript
DiskQuotaControl.GiveUserNameResolutionPriority(
  oUser
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*аусер* 
</dt> <dd>

Тип: **объект**

Выражение объекта, результатом которого является объект [**дидисккуотаусер**](didiskquotauser-object.md) пользователя.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Если включено асинхронное разрешение имен, объекты пользователя помещаются в очередь. По умолчанию они обслуживаются в том порядке, в котором они размещены в очереди. Метод **гивеусернамересолутионприорити** перемещает объект на передний план, чтобы он находящихся рядом в строке для обслуживания.

Чтобы включить асинхронное разрешение имен, используйте свойство [**усернамересолутион**](diskquotacontrol-usernameresolution.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                    |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Дсккуота. h</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 5,0 или более поздняя)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Дисккуотаконтрол**](diskquotacontrol-object.md)
</dt> </dl>

 

 




