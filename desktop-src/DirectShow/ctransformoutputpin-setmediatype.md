---
description: Ктрансформаутпутпин. Сетмедиатипе, метод Сетмедиатипе задает тип носителя для соединения.
ms.assetid: 1d6569c1-e27b-4e96-af5a-64a78b762afd
title: Ктрансформаутпутпин. Сетмедиатипе, метод (Трансфрм. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransformOutputPin.SetMediaType
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 5aa8dcfbf573f6ca5b047c9f84567a84985732c7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255328"
---
# <a name="ctransformoutputpinsetmediatype-method"></a>Ктрансформаутпутпин. Сетмедиатипе, метод

`SetMediaType`Метод задает тип носителя для соединения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetMediaType(
   const CMediaType *mt
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*машин* 
</dt> <dd>

Указатель на объект [**кмедиатипе**](cmediatype.md) , указывающий тип мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Комментарии

Этот метод переопределяет метод [**кбасепин:: сетмедиатипе**](cbasepin-setmediatype.md) . Он вызывает метод [**ктрансформфилтер:: сетмедиатипе**](ctransformfilter-setmediatype.md) фильтра для информирования фильтра.

Перед вызовом этого метода ПИН-код должен проверить, является ли тип носителя приемлемым.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




