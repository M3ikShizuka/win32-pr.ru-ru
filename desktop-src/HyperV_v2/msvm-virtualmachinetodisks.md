---
description: Настройка передачи данных в виде массива в \_ класс мсвм коллектионреференцепоинтекспортсеттингдата.
ms.assetid: f127880f-f917-4069-a283-a6f9427c5e07
title: Класс Msvm_VirtualMachineToDisks
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_VirtualMachineToDisks
- Msvm_VirtualMachineToDisks.VirtualMachineId
- Msvm_VirtualMachineToDisks.DisksToExport
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: b24c99d4e4c066122dbc26c79433668cd965a2bdcce13e3ceb319fb23a954fdf
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119899034"
---
# <a name="msvm_virtualmachinetodisks-class"></a>\_Класс мсвм виртуалмачинетодискс

Настройка передачи данных в виде массива в класс [**мсвм \_ коллектионреференцепоинтекспортсеттингдата**](msvm-collectionreferencepointexportsettingdata.md) .

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_VirtualMachineToDisks
{
  string VirtualMachineId;
  string DisksToExport[];
};
```

## <a name="members"></a>Члены

Класс **мсвм \_ виртуалмачинетодискс** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **мсвм \_ виртуалмачинетодискс** имеет следующие свойства.

<dl> <dt>

**дискстоекспорт**
</dt> <dd> <dl> <dt>

Тип данных: массив **строк**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Идентификаторы экземпляров WMI для дисков, которые относятся к заданному ИДЕНТИФИКАТОРу виртуальной машины, для которой необходимо экспортировать данные.

</dd> <dt>

**виртуалмачинеид**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: чтение и запись
</dt> </dl>

ИДЕНТИФИКАТОР виртуальной машины, с которой связаны виртуальные диски.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                             |
| Минимальная версия сервера<br/> | Windows Server 2016<br/>                                                                          |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



 

 




