---
description: 'Метод WebMethod извлекает количество буферов, которые будут созданы распределителем, и свойства буфера. Этот метод реализует метод Имемаллокатор:: Properties.'
ms.assetid: ccee4d69-52fc-4e3c-b6a4-787914708be4
title: Метод Кбасеаллокатор.-Properties (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseAllocator.GetProperties
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 469eb062113ab2ee87e6462b0e0227eaba11673a239794c844125823c4b8a05f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119832754"
---
# <a name="cbaseallocatorgetproperties-method"></a>Кбасеаллокатор... Properties, метод

`GetProperties`Метод получает количество буферов, которые будут созданы распределителем, и свойства буфера. Этот метод реализует метод [**имемаллокатор:: Properties**](/windows/desktop/api/Strmif/nf-strmif-imemallocator-getproperties) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetProperties(
   ALLOCATOR_PROPERTIES *pProps
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппропс* 
</dt> <dd>

Указатель на структуру [**\_ свойств распределителя**](/windows/win32/api/strmif/ns-strmif-allocator_properties) , которая получает свойства распределителя.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




