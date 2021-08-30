---
description: Определяет, можно ли перенести указанную виртуальную систему на целевой узел, заданный сетевым именем или IP-адресом.
ms.assetid: eacc8448-4683-48df-81b9-8599292944db
title: Метод Чекквиртуалсистемисмигратаблетохост класса Msvm_VirtualSystemMigrationService
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_VirtualSystemMigrationService.CheckVirtualSystemIsMigratableToHost
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: d5305ead7b84255524d87355596015a06d6dba7887ba028bdc5e677b4a9e6cd4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120041914"
---
# <a name="checkvirtualsystemismigratabletohost-method-of-the-msvm_virtualsystemmigrationservice-class"></a>Метод Чекквиртуалсистемисмигратаблетохост \_ класса Виртуалсистеммигратионсервице мсвм

Определяет, можно ли перенести указанную виртуальную систему на целевой узел, заданный сетевым именем или IP-адресом.

## <a name="syntax"></a>Синтаксис


```mof
uint32 CheckVirtualSystemIsMigratableToHost(
  [in]  Msvm_ComputerSystem REF ComputerSystem,
  [in]  string                  DestinationHost,
  [in]  string                  MigrationSettingData,
  [in]  string                  NewSystemSettingData,
  [in]  string                  NewResourceSettingData[],
  [out] boolean                 IsMigratable
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ComputerSystem* \[ окне\]
</dt> <dd>

Ссылка на экземпляр класса [**мсвм \_ ComputerSystem**](msvm-computersystem.md) , представляющий виртуальную машину для проверки возможности миграции.

</dd> <dt>

*Дестинатионхост* \[ окне\]
</dt> <dd>

Имя хостовой системы для миграции. Формат этого имени задается свойством **дестинатионхостформатссуппортед** класса [**мсвм \_ виртуалсистеммигратионкапабилитиес**](msvm-virtualsystemmigrationcapabilities.md) , связанного с этим классом.

</dd> <dt>

*Мигратионсеттингдата* \[ окне\]
</dt> <dd>

Встроенный экземпляр класса [**мсвм \_ виртуалсистеммигратионсеттингдата**](msvm-virtualsystemmigrationsettingdata.md) , представляющий параметры для операции миграции.

</dd> <dt>

*Невсистемсеттингдата* \[ окне\]
</dt> <dd>

Встроенный экземпляр класса [**мсвм \_ виртуалсистемсеттингдата**](msvm-virtualsystemsettingdata.md) , представляющий новые свойства, применимые к виртуальной системе после переноса.

</dd> <dt>

*Невресаурцесеттингдата* \[ окне\]
</dt> <dd>

Массив строк, содержащий встроенный экземпляр класса [**мсвм \_ ресаурцеаллокатионсеттингдата**](msvm-resourceallocationsettingdata.md) , который представляет новые свойства, применимые к виртуальным ресурсам виртуальной системы после переноса.

</dd> <dt>

*Переносимость* \[ заполняет\]
</dt> <dd>

Получает результат проверки миграции, указывающий, можно ли успешно выполнить миграцию виртуальной системы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает одно из следующих значений.

<dl> <dt>

**Завершено без ошибок** (0)
</dt> <dt>

**Не поддерживается** (1)
</dt> <dt>

**Сбой** (2)
</dt> <dt>

**Время ожидания** (3)
</dt> <dt>

**Недопустимый параметр** (4)
</dt> <dt>

**Недопустимое состояние** (5)
</dt> <dt>

**Несовместимые параметры** (6)
</dt> <dt>

**Зарезервировано DMTF** (..)
</dt> <dt>

**Метод зарезервирован** (4097.. 32767)
</dt> <dt>

**Зависит от поставщика** (32768.65 535)
</dt> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                    |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Мсвм \_ виртуалсистеммигратионсервице**](msvm-virtualsystemmigrationservice.md)
</dt> </dl>

 

 




