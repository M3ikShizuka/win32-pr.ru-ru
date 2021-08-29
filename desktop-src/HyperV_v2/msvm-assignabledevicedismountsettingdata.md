---
description: Представляет параметры виртуальной системы для импорта. Используется методом Dismount \_ класса мсвм ассигнабледевицесервице.
ms.assetid: 49892e21-3e8d-4644-8cde-72966927f350
title: Класс Msvm_AssignableDeviceDismountSettingData
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_AssignableDeviceDismountSettingData
- Msvm_AssignableDeviceDismountSettingData.DeviceInstancePath
- Msvm_AssignableDeviceDismountSettingData.DeviceLocationPath
- Msvm_AssignableDeviceDismountSettingData.RequireAcsSupport
- Msvm_AssignableDeviceDismountSettingData.RequireDeviceMitigations
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: 67d2bf61cc317fee3dd04e464384020cfa04be9f601205e44d031c4fe4fa3ff8
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119693494"
---
# <a name="msvm_assignabledevicedismountsettingdata-class"></a>\_Класс мсвм ассигнабледевицедисмаунтсеттингдата

Представляет параметры виртуальной системы для импорта. Используется методом [**dismount**](msvm-assignabledeviceservice-dismountassignabledevice.md) класса [**мсвм \_ ассигнабледевицесервице**](msvm-assignabledeviceservice.md) .

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[AMENDMENT]
class Msvm_AssignableDeviceDismountSettingData : CIM_SettingData
{
  string  DeviceInstancePath;
  string  DeviceLocationPath;
  boolean RequireAcsSupport;
  boolean RequireDeviceMitigations;
};
```

## <a name="members"></a>Члены

Класс **мсвм \_ ассигнабледевицедисмаунтсеттингдата** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **мсвм \_ ассигнабледевицедисмаунтсеттингдата** имеет следующие свойства.

<dl> <dt>

**девицеинстанцепас**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: чтение и запись
</dt> </dl>

Идентификатор экземпляра устройства PNP.

</dd> <dt>

**девицелокатионпас**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: чтение и запись
</dt> </dl>

Путь расположения устройства PNP.

</dd> <dt>

**рекуиреакссуппорт**
</dt> <dd> <dl> <dt>

Тип данных: **логический**
</dt> <dt>

Тип доступа: чтение и запись
</dt> </dl>

Указывает, должна ли обязательная поддержка ACS быть выполнена перед отключением.

</dd> <dt>

**рекуиредевицемитигатионс**
</dt> <dd> <dl> <dt>

Тип данных: **логический**
</dt> <dt>

Тип доступа: чтение и запись
</dt> </dl>

Указывает, должны ли быть решены устройства перед отключением.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1703\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows Server 2016<br/>                                                                          |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_SETTINGDATA CIM**](cim-settingdata.md)
</dt> </dl>

 

 




