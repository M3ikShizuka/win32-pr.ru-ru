---
description: Возвращает значение FALSE, если текущий поток является владельцем указанной критической секции.
ms.assetid: 1a2cb56c-2806-4bb2-b904-985af332b290
title: Функция Критчеккаут (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CritCheckOut
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fb1289bd89771797be88220f49d8af6f468a11c54e9954c32786e3af72dc1956
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119908094"
---
# <a name="critcheckout-function"></a>Функция Критчеккаут

Возвращает **значение false** , если текущий поток является владельцем указанной критической секции.

## <a name="syntax"></a>Синтаксис


```C++
BOOL WINAPI CritCheckOut(
   CCritSec *pcCrit
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пккрит* 
</dt> <dd>

Указатель на критический раздел [**ккритсек**](ccritsec.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

В отладочных сборках возвращает **значение false** , если текущий поток является владельцем этой критической секции, или **true** в противном случае. В розничных сборках всегда возвращает **значение true**.

## <a name="remarks"></a>Remarks

Эта функция является инверсией функции [**критчеккин**](critcheckin.md) . Если **критчеккин** возвращает **значение true**, **критчеккаут** возвращает **значение false** и наоборот.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Функции отладки критического раздела](critical-section-debugging-functions.md)
</dt> </dl>

 

 




