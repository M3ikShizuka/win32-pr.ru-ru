---
description: Структура ХАНДОФФТАБЛЕ определяет протоколы переданной таблицы.
ms.assetid: 6bb7465b-c1ba-4ffe-aecf-8125993c309a
title: Структура ХАНДОФФТАБЛЕ (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- HANDOFFTABLE
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: 842ef9fde56ff6b4c420034b861aa8c151e7e6b8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067608"
---
# <a name="handofftable-structure"></a>Структура ХАНДОФФТАБЛЕ

Структура **хандоффтабле** определяет протоколы переданной таблицы.

Эта структура заполняется сетевой монитор на основе информации в предоставленном пользователем .ini файле, предоставленном при вызове функции [**креатехандоффтабле**](createhandofftable.md) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct HANDOFFTABLE {
  DWORD          hot_sig;
  DWORD          hot_NumEntries;
  LPHANDOFFENTRY hot_Entries;
} HANDOFFTABLE, *LPHANDOFFTABLE;
```



## <a name="members"></a>Участники

<dl> <dt>

**Горячая \_ подпись**
</dt> <dd>

Сигнатура, которая идентифицирует эту таблицу как таблицу переданных.

</dd> <dt>

**горячий \_ нументриес**
</dt> <dd>

Число записей, которые сетевой монитор добавить в таблицу передачи.

</dd> <dt>

**горячий \_ записи**
</dt> <dd>

Таблица передачи.

</dd> </dl>

## <a name="remarks"></a>Remarks

Эта структура и связанные с ней структуры ХАНДОФФЕНТРИ заполняются с помощью сетевой монитор, когда сетевой монитор создает таблицу передачи.

Сведения о протоколе, используемые при создании таблицы передачи, предоставляются в файле .ini, предоставляемом приложением при вызове [**креатехандоффтабле**](createhandofftable.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[хандоффентри](handoffentry.md)
</dt> <dt>

[креатехандоффтабле](createhandofftable.md)
</dt> </dl>

 

 




