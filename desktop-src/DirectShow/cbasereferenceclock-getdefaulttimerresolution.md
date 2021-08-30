---
description: Метод Жетдефаулттимерресолутион возвращает текущее разрешение таймера ссылочного времени.
ms.assetid: 14176f9c-7fa1-47f6-a261-9c66e271a3f2
title: Кбасереференцеклокк. Жетдефаулттимерресолутион, метод (Рефклокк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseReferenceClock.GetDefaultTimerResolution
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: dbd3eb192839d6957af9fb63c32a1b1dcbb3a5c386c47d2f66408ec63d7cba21
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120076572"
---
# <a name="cbasereferenceclockgetdefaulttimerresolution-method"></a>Кбасереференцеклокк. Жетдефаулттимерресолутион, метод

`GetDefaultTimerResolution`Метод возвращает текущее разрешение таймера ссылочного времени.

## <a name="syntax"></a>Синтаксис


```C++
STDMETHODIMP GetDefaultTimerResolution(
   REFERENCE_TIME *pTimerResolution
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*птимерресолутион* 
</dt> <dd>

Получает запрошенное разрешение таймера в единицах 100-наносекундных.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Этот метод реализует метод [**иреференцеклокктимерконтрол:: жетдефаулттимерресолутион**](/windows/desktop/api/Strmif/nf-strmif-ireferenceclocktimercontrol-getdefaulttimerresolution) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>рефклокк. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасереференцеклокк**](cbasereferenceclock.md)
</dt> </dl>

 

 




