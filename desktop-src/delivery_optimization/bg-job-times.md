---
title: Структура BG_JOB_TIMES (Deliveryoptimization. h)
description: Структура BG_JOB_TIMES предоставляет штампы времени, связанные с заданием.
ms.assetid: 0147478F-C850-4B66-AB15-042C1A81D6B5
keywords:
- Структура BG_JOB_TIMES
topic_type:
- apiref
api_name:
- BG_JOB_TIMES
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 4b0fe36c9994bc03a807ff4a575945d203b1f62391b498cca094ed8f264be684
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119793405"
---
# <a name="bg_job_times-structure"></a>Структура BG_JOB_TIMES

Структура **BG_JOB_TIMES** предоставляет штампы времени, связанные с заданием.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _BG_JOB_TIMES {
  FILETIME CreationTime;
  FILETIME ModificationTime;
  FILETIME TransferCompletionTime;
} BG_JOB_TIMES;
```



## <a name="members"></a>Члены

<dl> <dt>

**CreationTime**
</dt> <dd>

Время создания задания. Время указывается в виде [fileTime](/windows/win32/api/minwinbase/ns-minwinbase-filetime).

</dd> <dt>

**модификатионтиме**
</dt> <dd>

Время последнего изменения задания или передачи байтов. Изменение этого значения осуществляется путем добавления файлов или вызова любого из методов Set в интерфейсах [ * *использованием метода ibackgroundcopyjob \** _](/previous-versions//mt811348(v=vs.85)) . Кроме того, изменения в состоянии задания и вызов методов [_ *Suspend* *](ibackgroundcopyjob-suspend.md), [**Resume**](ibackgroundcopyjob-resume.md), [**Cancel**](ibackgroundcopyjob-cancel.md)и [**Complete**](ibackgroundcopyjob-complete.md) изменяют это значение. Время указывается в виде [fileTime](/windows/win32/api/minwinbase/ns-minwinbase-filetime).

</dd> <dt>

**трансферкомплетионтиме**
</dt> <dd>

Время, когда задание перешло в состояние BG_JOB_STATE_TRANSFERRED. Время указывается в виде [fileTime](/windows/win32/api/minwinbase/ns-minwinbase-filetime).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Использованием метода ibackgroundcopyjob:: навремя**](ibackgroundcopyjob-gettimes.md)
</dt> </dl>

 

