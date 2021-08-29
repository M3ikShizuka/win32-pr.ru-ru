---
description: Метод Локкмедиа класса Msvm_DisketteDrive — блокирует или освобождает носитель.
ms.assetid: 90f7e06c-92d0-4742-a74d-68ae6bfc00bf
title: Метод Локкмедиа класса Msvm_DisketteDrive
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_DisketteDrive.LockMedia
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: 31cdddccf5a62c5f26f83351977090fa5c5a33e24476a3de4e88ee5e40938f8d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119431034"
---
# <a name="lockmedia-method-of-the-msvm_diskettedrive-class"></a>Метод Локкмедиа \_ класса Дискеттедриве мсвм

Блокирует или освобождает носитель.

## <a name="syntax"></a>Синтаксис


```mof
uint32 LockMedia(
  [in] boolean Lock
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Блокировка* \[ окне\]
</dt> <dd>

**значение true** , чтобы заблокировать носитель; **значение false** , чтобы освободить носитель.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 в случае успешного выполнения; в противном случае возвращает одно из следующих значений:

<dl> <dt>

**Завершено без ошибок** (0)
</dt> <dt>

**Не поддерживается** (1)
</dt> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1<br/>                                                                                  |
| Минимальная версия сервера<br/> | Windows Server 2012 R2<br/>                                                                       |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Мсвм \_ дискеттедриве**](msvm-diskettedrive.md)
</dt> </dl>

 

 




