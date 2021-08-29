---
description: Структура PF \_ хандоффсет определяет протоколы, которые передаются средству синтаксического анализа, или протоколы, к которым он передает.
ms.assetid: 2fda399d-a09e-47b4-bb2e-95996de9f950
title: Структура PF_HANDOFFSET (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PF_HANDOFFSET
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: 68e3f3608ac1aeff0f6d54ee7c94c39b76b0df08bb7dc41b05063f9cf53c48a2
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120036844"
---
# <a name="pf_handoffset-structure"></a>\_Структура PF хандоффсет

Структура **PF \_ хандоффсет** определяет протоколы, которые передаются средству синтаксического анализа, или протоколы, к которым он передает.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PF_HANDOFFSET {
  DWORD           nEntries;
  PF_HANDOFFENTRY Entry[];
} PF_HANDOFFSET, *PPF_HANDOFFSET;
```



## <a name="members"></a>Члены

<dl> <dt>

**нентриес**
</dt> <dd>

Число протоколов.

</dd> <dt>

**Ввод**
</dt> <dd>

Массив структур [PF \_ хандоффентри](pf-handoffentry.md) , определяющий каждый протокол.

</dd> </dl>

## <a name="remarks"></a>Remarks

Структура [PF \_ парсеринфо](pf-parserinfo.md) использует структуру **PF \_ хандоффсет** для перечисления следующих целей:

-   Какие протоколы передаются средству синтаксического анализа.
-   Протоколы, к которым средство синтаксического анализа передает.

Структура **PF \_ хандоффсет** должна быть выделена с помощью **хеапаллок**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[PF \_ парсеринфо](pf-parserinfo.md)
</dt> <dt>

[PF \_ хандоффентри](pf-handoffentry.md)
</dt> </dl>

 

 




