---
description: Структура PF \_ фолловентри определяет протокол, который сетевой монитор добавляется в следующий набор средства синтаксического анализа.
ms.assetid: 931ae70f-8c5e-4b7a-aae6-64a33dac3b23
title: Структура PF_FOLLOWENTRY (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PF_FOLLOWENTRY
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: f93ec4784fc8d0f92f68fdff3914e230ffd3cdce
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067564"
---
# <a name="pf_followentry-structure"></a>\_Структура PF фолловентри

Структура **PF \_ фолловентри** определяет протокол, который сетевой монитор добавляется в следующий набор средства синтаксического анализа.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PF_FOLLOWENTRY {
  char szProtocol[MAX_PROTOCOL_NAME_LEN];
} PF_FOLLOWENTRY, *PPF_FOLLOWENTRY;
```



## <a name="members"></a>Участники

<dl> <dt>

**сзпротокол**
</dt> <dd>

Имя протокола.

</dd> </dl>

## <a name="remarks"></a>Remarks

В [структуре \_ следов PF](pf-followset.md) используется массив структур **PF \_ фолловентри** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[\_следующий PF](pf-followset.md)
</dt> </dl>

 

 




