---
description: Представляет устройство связи для беспроводной локальной сети, которое соответствует серии спецификаций IEEE 802,11.
ms.assetid: c4e3345f-5c7d-4d1d-9a94-64112d7334ff
title: Класс CIM_WiFiPort
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CIM_WiFiPort
- CIM_WiFiPort.Speed
- CIM_WiFiPort.MaxSpeed
- CIM_WiFiPort.PortType
- CIM_WiFiPort.PermanentAddress
- CIM_WiFiPort.NetworkAddresses
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: a03b1fa986bbd03dd786678c57bd8896ec927ab707205d56e0889d9f2dc2be48
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119427644"
---
# <a name="cim_wifiport-class"></a>\_Класс CIM вифипорт

Представляет устройство связи для беспроводной локальной сети, которое соответствует серии спецификаций IEEE 802,11.

## <a name="syntax"></a>Синтаксис

``` syntax
[Abstract, Version("2.22.0"), UMLPackagePath("CIM::Device::Ports"), AMENDMENT]
class CIM_WiFiPort : CIM_NetworkPort
{
  uint64 Speed;
  uint64 MaxSpeed;
  uint16 PortType;
  string PermanentAddress;
  string NetworkAddresses[];
};
```

## <a name="members"></a>Члены

Класс **CIM \_ вифипорт** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **CIM \_ вифипорт** имеет следующие свойства.

<dl> <dt>

**максспид**
</dt> <dd> <dl> <dt>

Тип данных: **UInt64**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**override**](/windows/desktop/WmiSdk/standard-qualifiers) ("максспид")
</dt> </dl>

Максимальная поддерживаемая пропускная способность (в битах в секунду) на основе режима работы, указанного в свойстве **portType** . Например, **максспид** имеет значение "11000000", если **PortType** содержит "71" (802.11 b).

</dd> <dt>

**NetworkAddresses**
</dt> <dd> <dl> <dt>

Тип данных: массив **строк**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**override**](/windows/desktop/WmiSdk/standard-qualifiers) ("NetworkAddresses")
</dt> </dl>

Массив, содержащий MAC-адреса в стандарте IEEE 802 EUI-48. MAC-адрес имеет формат, состоящий из двенадцати шестнадцатеричных цифр, каждая из которых представляет один из шести октетов MAC-адреса в каноническом порядке.

</dd> <dt>

**перманентаддресс**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**override**](/windows/desktop/WmiSdk/standard-qualifiers) ("перманентаддресс")
</dt> </dl>

MAC-адрес порта IEEE 802 EUI-48. MAC-адрес имеет формат, состоящий из двенадцати шестнадцатеричных цифр, каждая из которых представляет один из шести октетов MAC-адреса в каноническом порядке.

</dd> <dt>

**Порта**
</dt> <dd> <dl> <dt>

Тип данных: **UInt16**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**override**](/windows/desktop/WmiSdk/standard-qualifiers) ("PortType")
</dt> </dl>

Режим работы 802,11, включенный для порта.

<dt>

<span id="Unknown"></span><span id="unknown"></span><span id="UNKNOWN"></span>

**Неизвестно** (0)


</dt> <dd></dd> <dt>

<span id="Other"></span><span id="other"></span><span id="OTHER"></span>

**Другое** (1)


</dt> <dd></dd> <dt>

<span id="802.11a"></span><span id="802.11A"></span>

**802.11 a** (70)


</dt> <dd></dd> <dt>

<span id="802.11b"></span><span id="802.11B"></span>

**802.11 b** (71)


</dt> <dd></dd> <dt>

<span id="802.11g"></span><span id="802.11G"></span>

**802.11 g** (72)


</dt> <dd></dd> <dt>

<span id="802.11n"></span><span id="802.11N"></span>

**802.11 n** (73)


</dt> <dd></dd> <dt>

<span id="DMTF_Reserved"></span><span id="dmtf_reserved"></span><span id="DMTF_RESERVED"></span>

**Зарезервировано DMTF** (..)


</dt> <dd></dd> <dt>

<span id="Vendor_Reserved"></span><span id="vendor_reserved"></span><span id="VENDOR_RESERVED"></span>

**Поставщик зарезервирован** (16000...)


</dt> <dd></dd> </dl>

</dd> <dt>

**Скорость**
</dt> <dd> <dl> <dt>

Тип данных: **UInt64**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**override**](/windows/desktop/WmiSdk/standard-qualifiers) ("скорость")
</dt> </dl>

Скорость передачи данных, с которой была получена текущая единица данных протокола ППДУ (ПЛКП (протокол конвергенции физических уровней), в битах в секунду. Это значение кодируется в первых 4 битах заголовка ПЛКП в каждом кадре ПЛКП.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                                    |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                                          |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_НЕТВОРКПОРТ CIM**](cim-networkport.md)
</dt> </dl>

 

