---
description: Метод Жетнексти извлекает элемент в указанной позиции и перемещает позицию.
ms.assetid: 3ec217ec-b0f9-4ff4-bdb7-ac204df99010
title: Кбаселист. Жетнексти, метод (Вкслист. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseList.GetNextI
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: b45556c1657961bdebf378f7e3908501f0bf5b971cf0c6533a55477b05a40ad9
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119983513"
---
# <a name="cbaselistgetnexti-method"></a>Кбаселист. Жетнексти, метод

`GetNextI`Метод получает элемент в указанной позиции и перемещает позицию.

## <a name="syntax"></a>Синтаксис


```C++
void* GetNextI(
  [ref] POSITION &rp
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*RP* \[ ЗНАЧ\]
</dt> <dd>

Ссылка на значение должности.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на элемент. Если значение *RP* равно **null**, метод возвращает **значение NULL**.

## <a name="remarks"></a>Remarks

Этот метод перемещает индикатор положения на следующую позицию. Если индикатор позиции перемещается за концом списка, метод присваивает ему **значение NULL**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вкслист. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбаселист**](cbaselist.md)
</dt> </dl>

 

 




