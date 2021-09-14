---
description: Метод конструктора Кмедиасампле. Кмедиасампле.
ms.assetid: 3ee67cfd-a968-4b7c-9c7b-1c28ddb9c343
title: Конструктор Кмедиасампле. Кмедиасампле (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaSample.CMediaSample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 0fd2601b9f53e8f79d9231dd34054932bec4e671
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055585"
---
# <a name="cmediasamplecmediasample-constructor"></a>Кмедиасампле. Кмедиасампле, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CMediaSample(
   TCHAR          *pName,
   CBaseAllocator *pAllocator,
   HRESULT        *phr,
   LPBYTE         pBuffer = NULL,
   LONG           length = 0
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pName* 
</dt> <dd>

Не обрабатывается.

</dd> <dt>

*паллокатор* 
</dt> <dd>

Указатель на объект [**кбасеаллокатор**](cbaseallocator.md) , который создал этот образец.

</dd> <dt>

*фр* 
</dt> <dd>

Не обрабатывается.

</dd> <dt>

*pBuffer* 
</dt> <dd>

Указатель на буфер памяти, выделенный вызывающим объектом, *длиной* размера.

</dd> <dt>

*length* 
</dt> <dd>

Длина буфера памяти.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Базовый класс не изменяет значение **HRESULT** , передаваемое в параметре *фр* .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиасампле**](cmediasample.md)
</dt> </dl>

 

 




