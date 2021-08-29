---
description: 'Метод SetProperties задает количество выделяемых буферов и размер каждого буфера. Этот метод переопределяет метод Кбасеаллокатор:: SetProperties.'
ms.assetid: 8d419432-a9a7-44fb-b916-8dacd08eb6ec
title: Цимажеаллокатор. SetProperties, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImageAllocator.SetProperties
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 1924db012ece5ad475a26e75315254ab5228c9cd50aa1dac74d39430f976a367
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119768214"
---
# <a name="cimageallocatorsetproperties-method"></a>Цимажеаллокатор. SetProperties, метод

`SetProperties`Метод задает количество выделяемых буферов и размер каждого буфера. Этот метод переопределяет метод [**кбасеаллокатор:: SetProperties**](cbaseallocator-setproperties.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetProperties(
   ALLOCATOR_PROPERTIES *pRequest,
   ALLOCATOR_PROPERTIES *pActual
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*предпоручение* 
</dt> <dd>

Указатель на структуру [**\_ свойств распределителя**](/windows/win32/api/strmif/ns-strmif-allocator_properties) , которая содержит требования к буферу.

</dd> <dt>

*пактуал* 
</dt> <dd>

Указатель на структуру **\_ свойств распределителя** , которая получает фактические свойства буфера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Этот метод вызывает [**Цимажеаллокатор:: чекксизес**](cimageallocator-checksizes.md) для проверки запрошенного размера буфера. Он также вызывает версию базового класса `SetProperties` .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Цимажеаллокатор**](cimageallocator.md)
</dt> </dl>

 

 




