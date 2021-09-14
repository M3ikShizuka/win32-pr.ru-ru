---
description: Метод Креатеимажесампле создает пример носителя.
ms.assetid: dae71692-5cbc-4bc7-a363-41766ef17c58
title: Цимажеаллокатор. Креатеимажесампле, метод (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CImageAllocator.CreateImageSample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 57463a7025ea816b6fe6bcaa8b964231458903de
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170032"
---
# <a name="cimageallocatorcreateimagesample-method"></a>Цимажеаллокатор. Креатеимажесампле, метод

`CreateImageSample`Метод создает пример носителя.

## <a name="syntax"></a>Синтаксис


```C++
virtual CImageSample* CreateImageSample(
   LPBYTE pData,
   LONG   Length
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pData* 
</dt> <dd>

Указатель на буфер *длины* размера, выделенный вызывающим объектом.

</dd> <dt>

*Длина* 
</dt> <dd>

Длина буфера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает объект [**Цимажесампле**](cimagesample.md) .

## <a name="remarks"></a>Remarks

Этот метод создает образец носителя, реализованный как объект **Цимажесампле** . Метод [**имедиасампле::-Point**](/windows/desktop/api/Strmif/nf-strmif-imediasample-getpointer) в примере возвращает указатель на буфер, указанный в параметре *pData* .

Если вы наследуете новый класс распределителя из [**Цимажеаллокатор**](cimageallocator.md) и новый пример класса Media из [**Цимажесампле**](cimagesample.md), следует переопределить этот метод, чтобы создать экземпляр класса-примера мультимедиа.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Цимажеаллокатор**](cimageallocator.md)
</dt> <dt>

[**Цимажеаллокатор:: Alloc**](cimageallocator-alloc.md)
</dt> </dl>

 

 




