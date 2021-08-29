---
description: Метод конструктора Ценуммедиатипес. Ценуммедиатипес.
ms.assetid: fae2e05c-3f7b-4511-9b9d-5a37ea03f851
title: Конструктор Ценуммедиатипес. Ценуммедиатипес (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CEnumMediaTypes.CEnumMediaTypes
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 189073bbf1f9c3f2d6475ecacacdbae7c7e7725bad392f726b9ee6faf0de3763
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120131304"
---
# <a name="cenummediatypescenummediatypes-constructor"></a>Ценуммедиатипес. Ценуммедиатипес, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CEnumMediaTypes(
   CBasePin        *pPin,
   CEnumMediaTypes *pEnumMediaTypes
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппин* 
</dt> <dd>

Указатель на ПИН-код, на котором должно быть выполнено перечисление.

</dd> <dt>

*пенуммедиатипес* 
</dt> <dd>

Указатель на интерфейс [**иенуммедиатипес**](/windows/desktop/api/Strmif/nn-strmif-ienummediatypes) перечислителя, который необходимо клонировать, или **значение NULL**.

</dd> </dl>

## <a name="remarks"></a>Remarks

Если *пенуммедиатипес* имеет **значение NULL**, этот метод инициализирует перечислитель до начала последовательности перечисления. В противном случае он дублирует внутреннее состояние перечислителя, заданного параметром *пенуммедиатипес*.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ценуммедиатипес**](cenummediatypes.md)
</dt> </dl>

 

 




