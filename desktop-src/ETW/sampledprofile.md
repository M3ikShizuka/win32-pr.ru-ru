---
description: Этот класс является классом типа события для выборки событий профиля. Следующий синтаксис упрощен из MOF-кода.
ms.assetid: 75ea1e5e-2554-40bb-aa9d-c6d4942c5801
title: Класс Сампледпрофиле
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SampledProfile
- SampledProfile.InstructionPointer
- SampledProfile.ThreadId
- SampledProfile.Count
api_type:
- NA
api_location: ''
ms.openlocfilehash: 52b0eeeff1c0640455b935cf1140ab285d937f35db02d098def39a60a06571a1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120041634"
---
# <a name="sampledprofile-class"></a>Класс Сампледпрофиле

Этот класс является классом типа события для выборки событий профиля.

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
[EventType{46}, EventTypeName{"SampleProfile"}]
class SampledProfile : PerfInfo
{
  uint32 InstructionPointer;
  uint32 ThreadId;
  uint32 Count;
};
```

## <a name="members"></a>Члены

Класс **сампледпрофиле** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **сампледпрофиле** имеет следующие свойства.

<dl> <dt>

**Количество**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (3)
</dt> </dl>

Не используется.

</dd> <dt>

**инструктионпоинтер**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (1), Pointer
</dt> </dl>

Адрес образа, который был запущен на момент выборки процессора.

</dd> <dt>

**Tидентификатор**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (2)
</dt> </dl>

Идентификатор потока, который был запущен на момент выборки процессора.

</dd> </dl>

## <a name="remarks"></a>Remarks

Эти события предоставляют примерный профиль выполнения. Событие записывает, что было выполнено на процессоре. События Image можно использовать для указания двоичного модуля, содержащего эту инструкцию. Затем эти сведения можно использовать для создания профиля выполнения в течение времени трассировки.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




