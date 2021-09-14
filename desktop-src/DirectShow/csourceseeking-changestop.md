---
description: Метод Чанжестоп вызывается при изменении позиции окончания.
ms.assetid: 3d4a73a4-68e6-449c-9637-62cad937c4b4
title: Ксаурцесикинг. Чанжестоп, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.ChangeStop
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: eefcc64b4692363c8caa8f39a3a0db9beb0d08b5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971614"
---
# <a name="csourceseekingchangestop-method"></a>Ксаурцесикинг. Чанжестоп, метод

`ChangeStop`Метод вызывается при изменении позиции окончания.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT ChangeStop() = 0;
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Метод [**ксаурцесикинг:: сетпоситионс**](csourceseeking-setpositions.md) вызывает этот метод, если позиция окончания изменяется. Этот метод является чисто виртуальным; производный класс должен реализовать его. В следующем примере показана возможная реализация:


```C++
HRESULT CMyStream::ChangeStop( )
{
    UpdateFromSeek();
    return S_OK;
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




