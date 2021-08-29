---
description: Структура ADDJOB \_ info \_ 1 определяет задание печати, а также каталог и файл, в котором приложение может сохранить это задание.
ms.assetid: de915932-11a7-47e8-9be9-edab76d94189
title: Структура ADDJOB_INFO_1 (Винспул. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ADDJOB_INFO_1
- _ADDJOB_INFO_1A
- _ADDJOB_INFO_1W
api_type:
- HeaderDef
api_location:
- Winspool.h
ms.openlocfilehash: 6a0abcd2d9d09b65e8b4d5dd27e01532859a8060eda7847f0c1b7888a3c9714f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119950764"
---
# <a name="addjob_info_1-structure"></a>\_Структура ADDJOB info \_ 1

Структура **ADDJOB \_ info \_ 1** определяет задание печати, а также каталог и файл, в котором приложение может сохранить это задание.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _ADDJOB_INFO_1 {
  LPTSTR Path;
  DWORD  JobId;
} ADDJOB_INFO_1, *PADDJOB_INFO_1;
```



## <a name="members"></a>Члены

<dl> <dt>

**Путь**
</dt> <dd>

Указатель на строку, завершающуюся нулем, которая содержит путь и имя файла, которые приложение может использовать для хранения задания печати.

</dd> <dt>

**JobId**
</dt> <dd>

Маркер задания печати.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>винспул. h (включает Windows. h)</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **\_ \_ Сведения о ADDJOB \_ 1W** (Юникод) и **\_ ADDJOB \_ info \_ 1A** (ANSI)<br/>                             |



## <a name="see-also"></a>См. также

<dl> <dt>

[Вывод на печать](printdocs-printing.md)
</dt> <dt>

[Структуры API диспетчера очереди печати](printing-and-print-spooler-structures.md)
</dt> <dt>

[**AddJob**](addjob.md)
</dt> </dl>

 

 




