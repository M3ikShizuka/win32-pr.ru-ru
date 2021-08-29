---
description: 'Метод Алтеркуалити уведомляет фильтр о том, что запрошено изменение качества. Этот метод переопределяет метод Ктрансформфилтер:: Алтеркуалити.'
ms.assetid: 9a1d1379-8557-4b33-ab49-b5c6a684f685
title: Квидеотрансформфилтер. Алтеркуалити, метод (Втранс. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CVideoTransformFilter.AlterQuality
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 6cd2568bfc9518e2eeaf0399fa53796e305d246c511e5ee5bea1d3a1cacf7712
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119998624"
---
# <a name="cvideotransformfilteralterquality-method"></a>Квидеотрансформфилтер. Алтеркуалити, метод

`AlterQuality`Метод уведомляет фильтр о запросе изменения качества. Этот метод переопределяет метод [**ктрансформфилтер:: алтеркуалити**](ctransformfilter-alterquality.md) .

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT AlterQuality(
   Quality q
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*формате* 
</dt> <dd>

Структура [**качества**](/windows/win32/api/strmif/ns-strmif-quality) , содержащая сообщение контроля качества.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение E \_ Fail.

## <a name="remarks"></a>Remarks

Этот метод вызывается, когда выходной ПИН-код получает качественное сообщение (с помощью метода [**икуалитиконтрол:: notify**](/windows/desktop/api/Strmif/nf-strmif-iqualitycontrol-notify) ).

Значение опоздания из *q* хранится в переменной-члене **m \_ итрлате** . Возвращаемое значение E \_ Fail означает, что модуль подготовки отчетов должен перехватить кадры, хотя класс **квидеотрансформфилтер** также будет удалять фреймы под правильными условиями.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>втранс. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Квидеотрансформфилтер**](cvideotransformfilter.md)
</dt> <dt>

[**Квидеотрансформфилтер:: Шаулдскипфраме**](cvideotransformfilter-shouldskipframe.md)
</dt> </dl>

 

 




