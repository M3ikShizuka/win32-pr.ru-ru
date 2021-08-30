---
description: Функция Екуалпинс проверяет, находятся ли два контакта на одном объекте.
ms.assetid: b6a92cb6-f4a9-4a14-831c-3b123e4692c0
title: Функция Екуалпинс (Вксутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- EqualPins
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: e304c8d9ed7ef94ee23280d1466450c73e0627d35183c7edfafc4ef13eeba636
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120079064"
---
# <a name="equalpins-function"></a>Функция Екуалпинс

Функция Екуалпинс проверяет, находятся ли два контакта на одном объекте.

## <a name="syntax"></a>Синтаксис


```C++
BOOL EqualPins(
   IUnknown *pPin1,
   IUnknown *pPin2
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pPin1* 
</dt> <dd>

Указатель на один ПИН-код.

</dd> <dt>

*pPin2* 
</dt> <dd>

Указатель на другой ПИН-код.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если оба контакта находятся в одном объекте, или **false** в противном случае.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксутил. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Различные вспомогательные функции](miscellaneous-helper-functions.md)
</dt> </dl>

 

 




