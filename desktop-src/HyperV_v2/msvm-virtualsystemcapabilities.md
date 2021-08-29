---
description: Описывает возможности связанной Мсвм \_ ComputerSystem.
ms.assetid: 7e3b51ba-f85d-4b83-abc6-a094d412eca1
title: Класс Msvm_VirtualSystemCapabilities
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_VirtualSystemCapabilities
- Msvm_VirtualSystemCapabilities.InstanceID
- Msvm_VirtualSystemCapabilities.Caption
- Msvm_VirtualSystemCapabilities.Description
- Msvm_VirtualSystemCapabilities.ElementName
- Msvm_VirtualSystemCapabilities.ElementNameEditSupported
- Msvm_VirtualSystemCapabilities.MaxElementNameLen
- Msvm_VirtualSystemCapabilities.RequestedStatesSupported
- Msvm_VirtualSystemCapabilities.ElementNameMask
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: 4b25f28c0ae75be9bc9b6cdb0ff752e99befb18131c758bd1ae461c909b1bf5c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119789214"
---
# <a name="msvm_virtualsystemcapabilities-class"></a>\_Класс мсвм виртуалсистемкапабилитиес

Описывает возможности связанной [**мсвм \_ ComputerSystem**](msvm-computersystem.md).

Следующий синтаксис является упрощенным MOF-файлным (MOF) кодом и включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_VirtualSystemCapabilities : CIM_EnabledLogicalElementCapabilities
{
  string  InstanceID;
  string  Caption = "Hyper-V Virtual System Capabilities";
  string  Description = "Defines Virtual System Capabilities";
  string  ElementName = "Hyper-V Virtual System Capabilities";
  boolean ElementNameEditSupported = True;
  unit16  MaxElementNameLen = 100;
  unit16  RequestedStatesSupported[];
  string  ElementNameMask;
};
```

## <a name="members"></a>Члены

Класс **мсвм \_ виртуалсистемкапабилитиес** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **мсвм \_ виртуалсистемкапабилитиес** имеет следующие свойства.

<dl> <dt>

**Caption**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Краткое описание объекта. Это свойство наследуется от [**CIM \_ манажеделемент**](/previous-versions/windows/desktop/iscsitarg/cim-managedelement).

</dd> <dt>

**Описание**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Описание объекта. Это свойство наследуется от [**CIM \_ манажеделемент**](/previous-versions/windows/desktop/iscsitarg/cim-managedelement).

</dd> <dt>

**ElementName**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Отображаемое имя объекта. Это свойство наследуется от [**CIM \_ манажеделемент**](/previous-versions/windows/desktop/iscsitarg/cim-managedelement).

</dd> <dt>

**елементнамидитсуппортед**
</dt> <dd> <dl> <dt>

Тип данных: **логический**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Указывает, можно ли изменить свойство **ElementName** . Это свойство наследуется от **CIM \_ енабледлогикалелементкапабилитиес**.

</dd> <dt>

**елементнамемаск**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Задает ограничения для **ElementName**, выраженные в виде регулярного выражения. Это свойство наследуется от **CIM \_ енабледлогикалелементкапабилитиес**.

</dd> <dt>

**InstanceID**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: **ключ**
</dt> </dl>

Уникально идентифицирует экземпляр этого класса. Это свойство наследуется от [**CIM \_ манажеделемент**](/previous-versions/windows/desktop/iscsitarg/cim-managedelement).

</dd> <dt>

**макселементнамелен**
</dt> <dd> <dl> <dt>

Тип данных: **unit16**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: **MaxValue** (256)
</dt> </dl>

Задает максимальную поддерживаемую длину свойства **ElementName** . Это свойство наследуется от **CIM \_ енабледлогикалелементкапабилитиес**.

</dd> <dt>

**рекуестедстатессуппортед**
</dt> <dd> <dl> <dt>

Тип данных: массив **unit16**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Указывает возможные состояния, которые могут быть запрошены при использовании метода **RequestStateChange** для включенного логического элемента. Это свойство наследуется от **CIM \_ енабледлогикалелементкапабилитиес**.



| Значение                                                                         | Значение              |
|-------------------------------------------------------------------------------|----------------------|
| <dl> <dt>2</dt> </dl>  | Активировано<br/>   |
| <dl> <dt>3</dt> </dl>  | Отключит<br/>  |
| <dl> <dt>4</dt> </dl>  | Завершение работы<br/> |
| <dl> <dt>6</dt> </dl>  | Автономная миграция<br/>   |
| <dl> <dt>7</dt> </dl>  | Тестирование<br/>      |
| <dl> <dt>8</dt> </dl>  | Которого<br/>     |
| <dl> <dt>9</dt> </dl>  | Замораживани<br/>   |
| <dl> <dt>10</dt> </dl> | Перезагрузка<br/>    |
| <dl> <dt>11</dt> </dl> | Reset<br/>     |



 

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                    |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



 

