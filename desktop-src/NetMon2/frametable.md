---
description: Структура ФРАМЕТАБЛЕ, круглый буфер указателей кадров, передается обратно в приложения, подключенные к интерфейсу ИТРК НПП.
ms.assetid: 6e2d4f8d-46f2-4d53-bc28-7b0706663490
title: Структура ФРАМЕТАБЛЕ (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- FRAMETABLE
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: 214a9e947c7aba34f0cc65d1df8d56a57b9d1087e168824494f64e30bd8098e8
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119890744"
---
# <a name="frametable-structure"></a>Структура ФРАМЕТАБЛЕ

Структура **фраметабле** , круглый буфер указателей кадров, передается обратно в приложения, подключенные к интерфейсу **итрк** НПП.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _FRAMETABLE {
  DWORD            FrameTableLength;
  DWORD            StartIndex;
  DWORD            EndIndex;
  DWORD            FrameCount;
  FRAME_DESCRIPTOR Frames[1];
} FRAMETABLE, *LPFRAMETABLE;
```



## <a name="members"></a>Члены

<dl> <dt>

**фраметаблеленгс**
</dt> <dd>

Общая длина таблицы.

</dd> <dt>

**StartIndex**
</dt> <dd>

Первый индекс в таблице.

</dd> <dt>

**EndIndex**
</dt> <dd>

Последний индекс в таблице.

</dd> <dt>

**FrameCount**
</dt> <dd>

Число кадров, описываемых этой таблицей.

</dd> <dt>

**Получен**
</dt> <dd>

Фактический массив дескрипторов кадров.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



 

 




