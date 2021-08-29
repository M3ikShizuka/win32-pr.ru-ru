---
title: Windows Типы данных сборщика событий (Евколл. h)
description: типы данных для сборщика событий Windows используются как типы переменных объектов подписки на события, типы параметров функций и типы возвращаемых функций.
ms.assetid: b78bdaf8-e034-40fe-acf8-632313e4fd94
ms.tgt_platform: multiple
keywords:
- EC_HANDLE
- EC_OBJECT_ARRAY_PROPERTY_HANDLE
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a8d0a3a0887fccebbd5cfb45042eaa59895febfa1001af93eed1161e9d33f8b0
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119620574"
---
# <a name="windows-event-collector-data-types"></a>Windows Типы данных сборщика событий

типы данных для сборщика событий Windows используются как типы переменных объектов подписки на события, типы параметров функций и типы возвращаемых функций.


```C++
typedef HANDLE EC_HANDLE;
typedef HANDLE EC_OBJECT_ARRAY_PROPERTY_HANDLE;
```



<dl> <dt>

**\_маркер EC**
</dt> <dd>

Обработчик для объекта подписки. Используется для представления подписки сборщика событий.

</dd> <dt>

**\_ \_ \_ маркер свойства массива объектов \_ EC**
</dt> <dd>

Обработайте массив значений свойств для источников событий подписки. Этот маркер массива возвращается методом [**екжетсубскриптионпроперти**](/windows/desktop/api/Evcoll/nf-evcoll-ecgetsubscriptionproperty) , когда значение **ексубскриптионевентсаурцес** передается в параметр *PropertyId* .

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>Евколл. h</dt> </dl> |



 

 





