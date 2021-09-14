---
description: '\_Структура схемы PID содержит определение содержимого идентификатора пакета транспортного потока MPEG-2.'
ms.assetid: c247ec75-483d-4587-a82f-07bbf6d277b4
title: Структура PID_MAP (Бдатипес. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PID_MAP
api_type:
- HeaderDef
api_location:
- bdatypes.h
ms.openlocfilehash: 98b238c61ccfcfb93e4ddcc0a051d9084228f604
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055436"
---
# <a name="pid_map-structure"></a>\_Структура схемы PID

`PID_MAP`Структура содержит определение содержимого идентификатора пакета транспортного потока MPEG-2.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  ULONG                ulPID;
  MEDIA_SAMPLE_CONTENT MediaSampleContent;
} PID_MAP;
```



## <a name="members"></a>Участники

<dl> <dt>

**улпид**
</dt> <dd>

Указывает идентификатор пакета (PID)

</dd> <dt>

**медиасамплеконтент**
</dt> <dd>

Задает содержимое полезных данных пакета в виде типа перечисления [**мультимедиа \_ образец \_ содержимого**](media-sample-content.md) .

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Бдатипес. h (включение Бдаифаце. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[DirectShow Сотрудник](directshow-structures.md)
</dt> <dt>

[**Интерфейс Иенумпидмап**](/previous-versions/windows/desktop/api/Bdaiface/nn-bdaiface-ienumpidmap)
</dt> </dl>

 

 




