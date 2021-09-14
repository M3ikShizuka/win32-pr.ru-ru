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
ms.openlocfilehash: ae5a888e619f6bed9cda203ccd8a197b0b25c001
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145038"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции отладки критического раздела](critical-section-debugging-functions.md)
</dt> </dl>

 

 




