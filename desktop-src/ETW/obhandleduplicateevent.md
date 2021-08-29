---
description: Представляет класс типа события для обработчика повторяющихся событий.
ms.assetid: a933ffaa-8c99-4b87-ad00-4c40fa4d8d26
title: Класс Обхандледупликативент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ObHandleDuplicateEvent
- ObHandleDuplicateEvent.Object
- ObHandleDuplicateEvent.ObjectType
- ObHandleDuplicateEvent.SourceHandle
- ObHandleDuplicateEvent.TargetHandle
- ObHandleDuplicateEvent.TargetProcessId
api_type:
- NA
api_location: ''
ms.openlocfilehash: 939d3c1b1e21d32b69f18e07a051fa0f9d0ab07e2c793425a576a200187306e5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120075264"
---
# <a name="obhandleduplicateevent-class"></a>Класс Обхандледупликативент

Представляет класс типа события для обработчика повторяющихся событий.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, EventType(34), EventTypeName("DuplicateHandle")]
class ObHandleDuplicateEvent : ObTrace
{
  uint32 Object;
  uint16 ObjectType;
  uint32 SourceHandle;
  uint32 TargetHandle;
  uint32 TargetProcessId;
};
```

## <a name="members"></a>Члены

Класс **обхандледупликативент** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **обхандледупликативент** имеет следующие свойства.

<dl> <dt>

**Объект**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Формат**](event-tracing-mof-qualifiers.md) ("x"), [**указатель**](event-tracing-mof-qualifiers.md), [**вмидатаид**](event-tracing-mof-qualifiers.md) (1)
</dt> </dl>

Объект.

</dd> <dt>

**ObjectType**
</dt> <dd> <dl> <dt>

Тип данных: **UInt16**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**вмидатаид**](event-tracing-mof-qualifiers.md) (5)
</dt> </dl>

Тип объекта.

</dd> <dt>

**саурцехандле**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Format**](event-tracing-mof-qualifiers.md) ("x"), [**вмидатаид**](event-tracing-mof-qualifiers.md) (2)
</dt> </dl>

Маркер исходного объекта.

</dd> <dt>

**таржесандле**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Format**](event-tracing-mof-qualifiers.md) ("x"), [**вмидатаид**](event-tracing-mof-qualifiers.md) (3)
</dt> </dl>

Маркер целевого объекта.

</dd> <dt>

**таржетпроцессид**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Format**](event-tracing-mof-qualifiers.md) ("x"), [**вмидатаид**](event-tracing-mof-qualifiers.md) (4)
</dt> </dl>

Идентификатор процесса целевого объекта.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                   |
| MOF<br/>                      | <dl> <dt>Вмикоре. mof</dt> </dl> |



 

 




