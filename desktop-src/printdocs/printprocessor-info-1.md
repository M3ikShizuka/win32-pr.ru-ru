---
description: В \_ структуре принтпроцессор info \_ 1 указывается имя установленного обработчика печати.
ms.assetid: 49b272c8-156b-4996-b3fd-92cde831f4ae
title: Структура PRINTPROCESSOR_INFO_1 (Винспул. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PRINTPROCESSOR_INFO_1
- _PRINTPROCESSOR_INFO_1A
- _PRINTPROCESSOR_INFO_1W
api_type:
- HeaderDef
api_location:
- Winspool.h
ms.openlocfilehash: 5ac35f85e904e9a80d9f244a1421b54fd0994a43
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343658"
---
# <a name="printprocessor_info_1-structure"></a>\_Структура принтпроцессор info \_ 1

В структуре **принтпроцессор \_ info \_ 1** указывается имя установленного обработчика печати.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PRINTPROCESSOR_INFO_1 {
  LPTSTR pName;
} PRINTPROCESSOR_INFO_1, *PPRINTPROCESSOR_INFO_1;
```



## <a name="members"></a>Участники

<dl> <dt>

**pName**
</dt> <dd>

Указатель на строку, завершающуюся нулем, которая указывает имя установленного обработчика печати.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>винспул. h (включает Windows. h)</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **\_ \_ Сведения о принтпроцессор \_ 1W** (Юникод) и **\_ принтпроцессор \_ info \_ 1A** (ANSI)<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Вывод на печать](printdocs-printing.md)
</dt> <dt>

[Структуры API диспетчера очереди печати](printing-and-print-spooler-structures.md)
</dt> <dt>

[**енумпринтпроцессорс**](enumprintprocessors.md)
</dt> </dl>

 

 




