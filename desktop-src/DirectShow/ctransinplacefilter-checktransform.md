---
description: 'Метод Чекктрансформ проверяет, совместим ли входной тип носителя с выходным типом носителя. Этот метод переопределяет метод Ктрансформфилтер:: Чекктрансформ.'
ms.assetid: d0953014-4a49-4738-a449-c247396a6794
title: Ктрансинплацефилтер. Чекктрансформ, метод (Трансип. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransInPlaceFilter.CheckTransform
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 6a80132723be0b70f2c4afe93306d7f581b7734c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255310"
---
# <a name="ctransinplacefilterchecktransform-method"></a>Ктрансинплацефилтер. Чекктрансформ, метод

`CheckTransform`Метод проверяет, совместим ли входной тип носителя с выходным типом носителя. Этот метод переопределяет метод [**ктрансформфилтер:: чекктрансформ**](ctransformfilter-checktransform.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CheckTransform(
   const CMediaType *mtIn,
   const CMediaType *mtOut
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*мтин* 
</dt> <dd>

Указатель на объект [**кмедиатипе**](cmediatype.md) , указывающий тип входных данных.

</dd> <dt>

*мтаут* 
</dt> <dd>

Указатель на объект **кмедиатипе** , указывающий тип выходных данных.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Комментарии

Фильтр **ктрансинплаце** никогда не вызывает `CheckTransform` . Вместо этого все соединения с ПИН-кодом используют [**ктрансформфилтер:: чеккинпуттипе**](ctransformfilter-checkinputtype.md) для проверки типа мультимедиа, предположение, что типы входных и выходных данных всегда совпадают.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансип. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ктрансинплацефилтер**](ctransinplacefilter.md)
</dt> </dl>

 

 




