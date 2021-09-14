---
description: Класс CIM \_ фруинклудеспродукт указывает, что заменяемое поле (FRU) может состоять из других продуктов.
ms.assetid: e57dc7f5-4c5b-4ec4-9300-e080053955cb
ms.tgt_platform: multiple
title: Класс CIM_FRUIncludesProduct
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CIM_FRUIncludesProduct
- CIM_FRUIncludesProduct.Component
- CIM_FRUIncludesProduct.FRU
api_type:
- DllExport
api_location:
- CIMWin32.dll
ms.openlocfilehash: 196f0cc1f2e81312e5e695c34e0a492ac7c05389
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126973061"
---
# <a name="cim_fruincludesproduct-class"></a>\_Класс CIM фруинклудеспродукт

Класс **CIM \_ фруинклудеспродукт** указывает, что заменяемое поле (FRU) может состоять из других продуктов.

> [!IMPORTANT]
> Классы CIM (модель CIM) в DMTF (распределенная задача управления) являются родительскими классами, на которых строятся классы WMI. В настоящее время WMI поддерживает только [схемы версии CIM 2. x](https://dmtf.org/standards/cim/schemas).

 

Приведенный ниже синтаксис является упрощенной версией кода MOF и включает все унаследованные свойства. Свойства перечислены в алфавитном порядке, а не в MOF.

## <a name="syntax"></a>Синтаксис

``` syntax
[Abstract, UUID("{87FEEDCA-DB2A-11d2-85FC-0000F8102E5F}"), Aggregation, Association, AMENDMENT]
class CIM_FRUIncludesProduct
{
  CIM_Product REF Component;
  CIM_FRU     REF FRU;
};
```

## <a name="members"></a>Участники

Класс **CIM \_ фруинклудеспродукт** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **CIM \_ фруинклудеспродукт** имеет следующие свойства.

<dl> <dt>

**Компонент**
</dt> <dd> <dl> <dt>

Тип данных: **\_ продукт CIM**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Ссылка на продукт, который является частью FRU.

</dd> <dt>

**ЭКСПЛУАТАЦИИ**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ FRU**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Aggregate**](/windows/desktop/WmiSdk/standard-qualifiers), [**Max**](/windows/desktop/WmiSdk/standard-qualifiers) (1)
</dt> </dl>

Ссылка на FRU.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Инструментарий WMI не реализует этот класс.

Эта документация является производной от описаний класса CIM, опубликованных в формате DMTF. Корпорация Майкрософт могла внести изменения в Исправление незначительных ошибок, соответствовать стандартам документации пакета Microsoft SDK или предоставить дополнительные сведения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



 

