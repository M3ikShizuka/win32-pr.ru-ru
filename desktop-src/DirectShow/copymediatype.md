---
description: Функция Копимедиатипе копирует \_ \_ в другую структуру структуру типа мультимедиа am, включая блок Format
ms.assetid: 5b47e197-abb5-4b2c-ad65-a506c5e239be
title: Функция Копимедиатипе (Мтипе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CopyMediaType
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 2e37f277244ae9b82c395d7901917e1fc1e78b35
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461957"
---
# <a name="copymediatype-function"></a>Функция Копимедиатипе

Функция **копимедиатипе** копирует в другую структуру структуру [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) , включая блок Format

## <a name="syntax"></a>Синтаксис


```C++
HRESULT WINAPI CopyMediaType(
         AM_MEDIA_TYPE *pmtTarget,
   const AM_MEDIA_TYPE *pmtSource
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пмттаржет* 
</dt> <dd>

Указатель на структуру [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) . Метод копирует тип мультимедиа в эту структуру.

</dd> <dt>

*пмтсаурце* 
</dt> <dd>

Указатель на источник — [**Структура \_ \_ типа мультимедиа**](/windows/win32/api/strmif/ns-strmif-am_media_type) для копирования.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает S \_ OK или E \_ OUTOFMEMORY.

## <a name="remarks"></a>Remarks

Эта функция выделяет память для блока Format. Если параметр *пмттаржет* уже содержит выделенный блок формата, произойдет утечка памяти. Чтобы избежать утечки памяти, вызовите [**фримедиатипе**](freemediatype.md) перед вызовом этой функции.

После возврата метода вызовите [**фримедиатипе**](freemediatype.md) для *пмттаржет* , чтобы освободить блок формата.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>мтипе. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Функции типа мультимедиа**](media-type-functions.md)
</dt> </dl>

 

 




