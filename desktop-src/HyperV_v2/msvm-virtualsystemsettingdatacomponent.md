---
description: Универсальная ассоциация, используемая для установления части отношений между одним экземпляром CIM \_ виртуалсистемсеттингдата и одним или несколькими экземплярами CIM \_ ресаурцеаллокатионсеттингдата.
ms.assetid: 936B41E7-1B3B-4A7B-86F0-E2F4497CE610
title: Класс Msvm_VirtualSystemSettingDataComponent
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_VirtualSystemSettingDataComponent
- Msvm_VirtualSystemSettingDataComponent.GroupComponent
- Msvm_VirtualSystemSettingDataComponent.PartComponent
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: 485ac065f91a83479081a3cddd89cbae5b6eaa95bc3a30733371075226f58cdd
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120083154"
---
# <a name="msvm_virtualsystemsettingdatacomponent-class"></a>\_Класс мсвм виртуалсистемсеттингдатакомпонент

Универсальная ассоциация, используемая для установления отношений "часть" между одним экземпляром [**CIM \_ виртуалсистемсеттингдата**](/previous-versions//cc136954(v=vs.85)) и одним или несколькими экземплярами [**CIM \_ ресаурцеаллокатионсеттингдата**](/previous-versions/windows/desktop/clushyperv/cim-resourceallocationsettingdata).

Следующий синтаксис является упрощенным MOF-файлным (MOF) кодом и включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[Association, Aggregation, Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_VirtualSystemSettingDataComponent : CIM_VirtualSystemSettingDataComponent
{
  CIM_VirtualSystemSettingData      REF GroupComponent;
  CIM_ResourceAllocationSettingData REF PartComponent;
};
```

## <a name="members"></a>Члены

Класс **мсвм \_ виртуалсистемсеттингдатакомпонент** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **мсвм \_ виртуалсистемсеттингдатакомпонент** имеет следующие свойства.

<dl> <dt>

**Ссылка**
</dt> <dd> <dl> <dt>

Тип данных: **[ **CIM \_ виртуалсистемсеттингдата**](/previous-versions//cc136954(v=vs.85))**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: **override**, **min** (1), **Max** (1)
</dt> </dl>

Родительский элемент в ассоциации. Это свойство наследуется от [**CIM \_ виртуалсистемсеттингдатакомпонент**](/previous-versions//cc150674(v=vs.85)).

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Тип данных: **[ **CIM \_ ресаурцеаллокатионсеттингдата**](/previous-versions/windows/desktop/clushyperv/cim-resourceallocationsettingdata)**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Дочерний элемент в ассоциации. Это свойство наследуется от [**CIM \_ виртуалсистемсеттингдатакомпонент**](/previous-versions//cc150674(v=vs.85)).

</dd> </dl>

## <a name="remarks"></a>Remarks

Доступ к классу **\_ виртуалсистемсеттингдатакомпонент мсвм** может быть ограничен фильтром контроля учетных записей. Дополнительные сведения см. в разделе [Управление учетными записями пользователей и инструментарий WMI](/windows/desktop/WmiSdk/user-account-control-and-wmi).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                    |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_ВИРТУАЛСИСТЕМСЕТТИНГДАТАКОМПОНЕНТ CIM**](cim-virtualsystemsettingdatacomponent.md)
</dt> <dt>

[**\_ВИРТУАЛСИСТЕМСЕТТИНГДАТАКОМПОНЕНТ CIM**](/previous-versions//cc150674(v=vs.85))
</dt> <dt>

[Классы виртуальных систем](virtual-system-classes.md)
</dt> </dl>

 

