---
description: Удаляет указанное отношение репликации виртуальной машины.
ms.assetid: 0D5013CE-7BAE-4A99-ABF2-F1ECC644A1B2
title: 'Метод Msvm_ReplicationService:: Ремоверепликатионрелатионшипекс'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_ReplicationService.RemoveReplicationRelationshipEx
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: de7dafaccca7ba9290a8dc3b696bd6aa1acea1b9808b080ab75b9c62f79d65f0
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119980054"
---
# <a name="msvm_replicationserviceremovereplicationrelationshipex-method"></a>Мсвм \_ репликатионсервице:: ремоверепликатионрелатионшипекс, метод

Удаляет указанное отношение репликации виртуальной машины.

## <a name="syntax"></a>Синтаксис


```C++
uint32 RemoveReplicationRelationshipEx(
  [in]  CIM_ComputerSystem ComputerSystem,
  [in]  string                 ReplicationRelationship,
  [out] CIM_ConcreteJob    Job
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ComputerSystem* \[ окне\]
</dt> <dd>

Ссылка на экземпляр [**CIM \_ ComputerSystem**](/windows/desktop/CIMWin32Prov/cim-computersystem) , представляющий виртуальную машину, для которой необходимо удалить репликацию.

</dd> <dt>

*Репликатионрелатионшип* \[ окне\]
</dt> <dd>

Строковое представление внедренного экземпляра класса [**мсвм \_ репликатионрелатионшип**](msvm-replicationrelationship.md) , определяющего отношение репликации для удаления.

</dd> <dt>

*Задание* \[ заполняет\]
</dt> <dd>

Если операция выполняется асинхронно, этот метод возвратит 4096, и этот параметр будет содержать ссылку на объект, производный от [**CIM \_ конкретежоб**](/previous-versions//cc136808(v=vs.85)). Если задача завершена, ссылка может иметь **значение NULL** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает одно из следующих значений.

<dl> <dt>

**Завершено без ошибок** (0)
</dt> <dt>

**Параметры метода проверены — задание запущено** (4096)
</dt> <dt>

**Сбой** (32768)
</dt> <dt>

**Отказано в доступе** (32769)
</dt> <dt>

**Не поддерживается** (32770)
</dt> <dt>

**Состояние неизвестно** (32771)
</dt> <dt>

**Время ожидания** (32772)
</dt> <dt>

**Недопустимый параметр** (32773)
</dt> <dt>

**Система используется** (32774)
</dt> <dt>

**Недопустимое состояние для этой операции** (32775)
</dt> <dt>

**Неверный тип данных** (32776)
</dt> <dt>

**Система недоступна** (32777)
</dt> <dt>

**Недостаточно памяти** (32778)
</dt> <dt>

**Файл не найден** (32779)
</dt> </dl>

## <a name="remarks"></a>Remarks

Для виртуальной машины реплики невозможно удалить первичную репликацию, если включена расширенная репликация.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                                 |
| Пространство имен<br/>                | \\\\Корневая \\ виртуализация \\ версии 2<br/>                                                                 |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**CreateReplicationRelationship**](createreplicationrelationship-msvm-replicationservice.md)
</dt> <dt>

[**Мсвм \_ репликатионсервице**](msvm-replicationservice.md)
</dt> </dl>

 

