---
description: Метод Сетабортсигнал задает флаг, который указывает, следует ли прерывать отрисовку и отклонять дальнейшие выборки.
ms.assetid: 2dbf3b4d-e285-4d17-a77c-01a16c09d148
title: Кбасерендерер. Сетабортсигнал, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.SetAbortSignal
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 70527d5e43ccab4df7b2110a33df8d813bd16d28
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254449"
---
# <a name="cbaserenderersetabortsignal-method"></a>Кбасерендерер. Сетабортсигнал, метод

`SetAbortSignal`Метод задает флаг, указывающий, следует ли прерывать отрисовку и отклонять дальнейшие выборки.

## <a name="syntax"></a>Синтаксис


```C++
void SetAbortSignal(
   BOOL bAbort
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*баборт* 
</dt> <dd>

Логическое значение, указывающее, следует ли прерывать подготовку к просмотру. Если **значение равно true**, то фильтр не будет отображать больше выборок.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод задает флаг [**кбасерендерер:: m \_ баборт**](cbaserenderer-m-babort.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




