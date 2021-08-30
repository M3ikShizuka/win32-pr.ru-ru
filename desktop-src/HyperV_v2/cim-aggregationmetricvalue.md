---
description: Представляет значение экземпляра метрики, определенной экземпляром CIM \_ аггрегатионметрикдефинитион.
ms.assetid: 663ef18a-0238-416f-9682-8809b271b4fc
title: Класс CIM_AggregationMetricValue
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CIM_AggregationMetricValue
- CIM_AggregationMetricValue.AggregationTimeStamp
- CIM_AggregationMetricValue.AggregationDuration
api_type:
- DllExport
api_location:
- vmms.exe
ms.openlocfilehash: 254b2325873c2037b50f6cc0b013865589c23e2197ca113dbcc41bae6dd8a352
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120041704"
---
# <a name="cim_aggregationmetricvalue-class"></a>\_Класс CIM аггрегатионметриквалуе

Представляет значение экземпляра метрики, определенной экземпляром **CIM \_ аггрегатионметрикдефинитион**.

## <a name="syntax"></a>Синтаксис

``` syntax
[Abstract, Version("2.22.0"), UMLPackagePath("CIM::Metrics::BaseMetric"), AMENDMENT]
class CIM_AggregationMetricValue : CIM_BaseMetricValue
{
  datetime AggregationTimeStamp;
  datetime AggregationDuration;
};
```

## <a name="members"></a>Члены

Класс **CIM \_ аггрегатионметриквалуе** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **CIM \_ аггрегатионметриквалуе** имеет следующие свойства.

<dl> <dt>

**аггрегатиондуратион**
</dt> <dd> <dl> <dt>

Тип данных: **DateTime**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**моделкорреспонденце**](/windows/desktop/WmiSdk/standard-qualifiers) ("**CIM \_ аггрегатионметриквалуе**.**Аггрегатионтиместамп**")
</dt> </dl>

Представляет период времени, в течение которого Вычисление агрегата было выполнено. Начало интервала мониторинга, по отношению к которому применяется статистическая функция, определяется путем вычитания значения **аггрегатиондуратион** из значения **аггрегатионтиместамп** .

</dd> <dt>

**аггрегатионтиместамп**
</dt> <dd> <dl> <dt>

Тип данных: **DateTime**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**моделкорреспонденце**](/windows/desktop/WmiSdk/standard-qualifiers) ("**CIM \_ аггрегатионметриквалуе**.**Duration (длительность**))
</dt> </dl>

Время, когда статистическая функция была применена для определения значения экземпляра метрики. Это отличается от времени создания экземпляра. Значение **аггрегатионтиместамп** изменяется каждый раз, когда статистическая функция применяется для вычисления значения.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                                    |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                                          |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_БАСЕМЕТРИКВАЛУЕ CIM**](cim-basemetricvalue.md)
</dt> </dl>

 

