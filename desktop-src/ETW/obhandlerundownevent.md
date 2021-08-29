---
description: Представляет класс типа событий для событий обработчиков объектов, связанных с началом и концом сбора данных.
ms.assetid: 96231819-f4ca-4c5c-bc19-4a76add5d3cf
title: Класс Обхандлерундовневент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ObHandleRundownEvent
- ObHandleRundownEvent.Handle
- ObHandleRundownEvent.Object
- ObHandleRundownEvent.ObjectName
- ObHandleRundownEvent.ObjectType
- ObHandleRundownEvent.ProcessId
api_type:
- NA
api_location: ''
ms.openlocfilehash: c901e0af73732656c71fe0af92cc4e7964c8fec1c59494fc68d0287182711873
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119900854"
---
# <a name="obhandlerundownevent-class"></a>Класс Обхандлерундовневент

Представляет класс типа событий для событий обработчиков объектов, связанных с началом и концом сбора данных. Это событие включает в себя перечисление всех дескрипторов при выполнении очистки.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, EventType{38,39}, EventTypeName{HandleDCStart,HandleDCEnd}]
class ObHandleRundownEvent : ObTrace
{
  uint32 Handle;
  uint32 Object;
  string ObjectName;
  uint16 ObjectType;
  uint32 ProcessId;
};
```

## <a name="members"></a>Члены

Класс **обхандлерундовневент** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **обхандлерундовневент** имеет следующие свойства.

<dl> <dt>

**Дескриптор**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Format**](event-tracing-mof-qualifiers.md) ("x"), [**вмидатаид**](event-tracing-mof-qualifiers.md) (3)
</dt> </dl>

Объектный обработчик.

</dd> <dt>

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

**ObjectName**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Format**](event-tracing-mof-qualifiers.md) ("w"), [**Стрингтерминатион**](event-tracing-mof-qualifiers.md) ("NullTerminated"), [**вмидатаид**](event-tracing-mof-qualifiers.md) (5)
</dt> </dl>

Имя объекта.

</dd> <dt>

**ObjectType**
</dt> <dd> <dl> <dt>

Тип данных: **UInt16**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**вмидатаид**](event-tracing-mof-qualifiers.md) (4)
</dt> </dl>

Тип объекта.

</dd> <dt>

**Идентификатор**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**Format**](event-tracing-mof-qualifiers.md) ("x"), [**вмидатаид**](event-tracing-mof-qualifiers.md) (2)
</dt> </dl>

Идентификатор процесса.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                   |
| MOF<br/>                      | <dl> <dt>Вмикоре. mof</dt> </dl> |



 

 




