---
description: '\_Структура следов PF определяет протоколы, которые могут предшествовать протоколу или следовать за ним.'
ms.assetid: ef444af9-edae-4547-9548-8a682c279f08
title: Структура PF_FOLLOWSET (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PF_FOLLOWSET
api_type:
- HeaderDef
api_location:
- Netmon.h
ms.openlocfilehash: f5c286d3b137df24f7da7f0fc5ae269a7a3d946d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146950"
---
# <a name="pf_followset-structure"></a>Общая папка PF, \_ Структура

Структура **\_ следов PF** определяет протоколы, которые могут предшествовать протоколу или следовать за ним.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _PF_FOLLOWSET {
  DWORD          nEntries;
  PF_FOLLOWENTRY Entry[];
} PF_FOLLOWSET, *PPF_FOLLOWSET;
```



## <a name="members"></a>Участники

<dl> <dt>

**нентриес**
</dt> <dd>

Число протоколов в списке.

</dd> <dt>

**Ввод**
</dt> <dd>

Массив структур [PF \_ фолловентри](pf-followentry.md) , описывающих каждый протокол.

</dd> </dl>

## <a name="remarks"></a>Remarks

Структура " [PF \_ парсеринфо](pf-parserinfo.md) " использует **структуру \_ следов PF** для перечисления протоколов, которые могут предшествовать или отслеживать протокол, обнаруженный анализатором.

Сетевой монитор использует сведения в структуре " **Общая \_ Папка** " для обновления следующих наборов конкретных анализаторов. Структура **\_ следов PF** должна быть выделена с помощью **хеапаллок**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[PF \_ фолловентри](pf-followentry.md)
</dt> <dt>

[PF \_ парсеринфо](pf-parserinfo.md)
</dt> </dl>

 

 




