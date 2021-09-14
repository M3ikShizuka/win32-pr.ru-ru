---
description: Функция Делетемедиатипе удаляет выделенную \_ \_ структуру типа файлов am, включая блок Format.
ms.assetid: 970f6b2b-2bf5-418d-b4ae-637561cd6765
title: Функция Делетемедиатипе (Мтипе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DeleteMediaType
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: db0de399ab1be7808370a6d0da57c4c3ca7b8de1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053491"
---
# <a name="deletemediatype-function"></a>Функция Делетемедиатипе

Функция **делетемедиатипе** удаляет выделенную структуру [**\_ \_ типа файлов AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) , включая блок Format.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI DeleteMediaType(
   AM_MEDIA_TYPE *pmt
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*состоит* 
</dt> <dd>

Указатель на структуру [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Комментарии

Эта функция используется для освобождения любой структуры типа мультимедиа, выделенной с помощью инструкции [**CoTaskMemAlloc**](/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemalloc) или [**креатемедиатипе**](createmediatype.md).

эта функция определена в библиотеке [DirectShow базовых классов](directshow-base-classes.md) . Если вы предпочитаете не ссылаться на библиотеку базовых классов, можно использовать следующий код:


```C++
// Release the format block for a media type.

void _FreeMediaType(AM_MEDIA_TYPE& mt)
{
    if (mt.cbFormat != 0)
    {
        CoTaskMemFree((PVOID)mt.pbFormat);
        mt.cbFormat = 0;
        mt.pbFormat = NULL;
    }
    if (mt.pUnk != NULL)
    {
        // pUnk should not be used.
        mt.pUnk->Release();
        mt.pUnk = NULL;
    }
}


// Delete a media type structure that was allocated on the heap.
void _DeleteMediaType(AM_MEDIA_TYPE *pmt)
{
    if (pmt != NULL)
    {
        _FreeMediaType(*pmt); 
        CoTaskMemFree(pmt);
    }
}
```





## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>мтипе. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**фримедиатипе**](freemediatype.md)
</dt> <dt>

[**Функции типа мультимедиа**](media-type-functions.md)
</dt> </dl>

 

