---
description: Кбасеаутпутпин. ДеЦидебуфферсизе, метод ДеЦидебуфферсизе задает требования к буферу.
ms.assetid: 1f7a3424-18ba-4a10-b09f-947ee8585ffa
title: Кбасеаутпутпин. ДеЦидебуфферсизе, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseOutputPin.DecideBufferSize
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 7a76f058e2f9c07a344453db87046704e26280a1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145081"
---
# <a name="cbaseoutputpindecidebuffersize-method"></a>Кбасеаутпутпин. ДеЦидебуфферсизе, метод

`DecideBufferSize`Метод задает требования к буферу.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT DecideBufferSize(
   IMemAllocator        *pAlloc,
   ALLOCATOR_PROPERTIES *ppropInputRequest
) = 0;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*паллок* 
</dt> <dd>

Указатель на интерфейс [**имемаллокатор**](/windows/desktop/api/Strmif/nn-strmif-imemallocator) распределителя.

</dd> <dt>

*ппропинпутрекуест* 
</dt> <dd>

Указатель на структуру [**\_ свойств распределителя**](/windows/win32/api/strmif/ns-strmif-allocator_properties) , которая содержит требования к буферу входного контакта. Если у входного контакта нет каких-либо требований, вызывающий объект должен обнулить члены этой структуры перед вызовом метода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК в случае успешного выполнения или **HRESULT** , указывающий на причину ошибки.

## <a name="remarks"></a>Remarks

Переопределите этот метод в производном классе. Вызовите метод [**имемаллокатор:: SetProperties**](/windows/desktop/api/Strmif/nf-strmif-imemallocator-setproperties) , чтобы указать требования к буферу. Как правило, производный класс будет учитывать требования к буферу входного контакта, но это не обязательно.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаутпутпин**](cbaseoutputpin.md)
</dt> </dl>

 

 




