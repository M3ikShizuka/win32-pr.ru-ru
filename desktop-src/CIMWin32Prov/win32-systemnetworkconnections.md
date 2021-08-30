---
description: '\_Класс WMI взаимосвязей Win32 системнетворкконнектионс связывает сетевое подключение и компьютерную систему, в которой он находится.'
ms.assetid: 7c47f653-74a9-4729-a72c-94930181f8c9
ms.tgt_platform: multiple
title: Класс Win32_SystemNetworkConnections
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_SystemNetworkConnections
- Win32_SystemNetworkConnections.GroupComponent
- Win32_SystemNetworkConnections.PartComponent
api_type:
- DllExport
api_location:
- CIMWin32.dll
ms.openlocfilehash: 8004ab6cecfec7ac17a0aee15e3b7869a2d35977901971f8b5dbf3790313c942
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119828024"
---
# <a name="win32_systemnetworkconnections-class"></a>\_Класс Win32 системнетворкконнектионс

[Класс WMI](../wmisdk/retrieving-a-class.md) взаимосвязей **Win32 \_ системнетворкконнектионс** связывает сетевое подключение и компьютерную систему, в которой он находится.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства. Свойства и методы имеют алфавитный порядок, а не порядок MOF.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, Provider("CIMWin32"), UUID("{8502C4F7-5FBB-11D2-AAC1-006008C78BC7}"), AMENDMENT]
class Win32_SystemNetworkConnections : CIM_SystemComponent
{
  Win32_ComputerSystem    REF GroupComponent;
  Win32_NetworkConnection REF PartComponent;
};
```

## <a name="members"></a>Члены

Класс **Win32 \_ системнетворкконнектионс** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **Win32 \_ системнетворкконнектионс** имеет следующие свойства.

<dl> <dt>

**Ссылка**
</dt> <dd> <dl> <dt>

Тип данных: **Win32 \_ ComputerSystem**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**ключ**](../wmisdk/key-qualifier.md), [**Переопределение**](../wmisdk/standard-qualifiers.md) ("GroupComponent"), [**маппингстрингс**](../wmisdk/standard-qualifiers.md) ("WMI \| Win32 \_ ComputerSystem")
</dt> </dl>

Ссылка на экземпляр, представляющий компьютерную систему, подключенную к сети.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Тип данных: **Win32 \_ NetworkConnection**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**ключ**](../wmisdk/key-qualifier.md), [**Переопределение**](../wmisdk/standard-qualifiers.md) ("PartComponent"), [**маппингстрингс**](../wmisdk/standard-qualifiers.md) ("WMI \| Win32 \_ NetworkConnection")
</dt> </dl>

Ссылка на экземпляр, представляющий сетевое подключение к данной компьютерной системе.

</dd> </dl>

## <a name="remarks"></a>Remarks

Класс **Win32 \_ системнетворкконнектионс** является производным от [**CIM \_ системкомпонент**](cim-systemcomponent.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_СИСТЕМКОМПОНЕНТ CIM**](cim-systemcomponent.md)
</dt> <dt>

[Классы операционной системы](./operating-system-classes.md)
</dt> </dl>

 

 
