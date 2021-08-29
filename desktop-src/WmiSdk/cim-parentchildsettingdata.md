---
description: Ассоциация между экземпляром CIM \_ виртуалсистемсеттингдата и \_ экземпляром CIM виртуалсистемсеттингдата, который представляет самый последний моментальный снимок, на основе которого основан этот объект.
ms.assetid: f6e93c22-077b-4604-8d0d-9584b1f4dce1
ms.tgt_platform: multiple
title: Класс CIM_ParentChildSettingData
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CIM_ParentChildSettingData
- Root\CIMV2.CIM_ParentChildSettingData.Antecedent
- Root\CIMV2.CIM_ParentChildSettingData.Dependent
- Root\CIMV2.CIM_ParentChildSettingData.Parent
- Root\CIMV2.CIM_ParentChildSettingData.Child
api_type:
- Schema
api_location:
- Root\CIMV2
ms.openlocfilehash: 2b6fa9dc11f7d5e17fbc74e24a079a56647bee37b7c0251a281b767797ab801c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119244664"
---
# <a name="cim_parentchildsettingdata-class"></a>\_Класс CIM парентчилдсеттингдата

Ассоциация между экземпляром [**CIM \_ виртуалсистемсеттингдата**](/previous-versions/windows/desktop/clushyperv/cim-virtualsystemsettingdata) и экземпляром **CIM \_ виртуалсистемсеттингдата** , который представляет самый последний моментальный снимок, на основе которого основан этот объект.

> [!IMPORTANT]
> Классы CIM (модель CIM) в DMTF (распределенная задача управления) являются родительскими классами, на которых строятся классы WMI. В настоящее время WMI поддерживает только [схемы версии CIM 2. x](https://dmtf.org/standards/cim/schemas).

 

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
class CIM_ParentChildSettingData : CIM_Dependency
{
  CIM_ManagedSystemElement     REF Antecedent;
  CIM_ManagedSystemElement     REF Dependent;
  CIM_VirtualSystemSettingData REF Parent;
  CIM_VirtualSystemSettingData REF Child;
};
```

## <a name="members"></a>Члены

Класс **CIM \_ парентчилдсеттингдата** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **CIM \_ парентчилдсеттингдата** имеет следующие свойства.

<dl> <dt>

**Завершил**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ манажедсистемелемент**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Ссылка на независимый объект в этой ассоциации.

Это свойство наследуется [**от \_ зависимости CIM**](/windows/desktop/CIMWin32Prov/cim-dependency).

</dd> <dt>

**Дочерний**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ виртуалсистемсеттингдата**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Данные параметра для виртуальной системы, представляющие дочерний элемент родительского элемента.

</dd> <dt>

**Него**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ манажедсистемелемент**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Ссылка на объект, который зависит от свойства **Antecedent** .

Это свойство наследуется [**от \_ зависимости CIM**](/windows/desktop/CIMWin32Prov/cim-dependency).

</dd> <dt>

**Родительский объект**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ виртуалсистемсеттингдата**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Данные параметра моментального снимка, на которых основаны данные дочернего параметра.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------|------------------------|
| Пространство имен<br/> | Корневой \\ CIMV2<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Зависимость CIM**](/windows/desktop/CIMWin32Prov/cim-dependency)
</dt> </dl>

 

