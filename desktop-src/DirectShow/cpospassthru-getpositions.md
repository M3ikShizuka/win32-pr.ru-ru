---
description: 'Метод Disposition извлекает текущую и заданную позиции относительно общей продолжительности потока. Этот метод реализует метод Имедиасикинг:: Disposition.'
ms.assetid: 51e45bc3-ae30-4b05-b9d9-684c1b028f51
title: Метод Кпоспасссру. Disposition (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CPosPassThru.GetPositions
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 0852199e8e143ce5b0348c3b79afd495a5a47627
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255472"
---
# <a name="cpospassthrugetpositions-method"></a>Метод Кпоспасссру. Disposition

`GetPositions`Метод получает текущую и заданную позиции относительно общей продолжительности потока. Этот метод реализует метод [**имедиасикинг:: Disposition**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-getpositions) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetPositions(
   LONGLONG *pCurrent,
   LONGLONG *pStop
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пкуррент* 
</dt> <dd>

Указатель на переменную, которая получает текущую координату в единицах текущего формата времени.

</dd> <dt>

*пстоп* 
</dt> <dd>

Указатель на переменную, которая получает точку окончания в единицах текущего формата времени.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** из подключенного ПИН-кода.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кпоспасссру**](cpospassthru.md)
</dt> </dl>

 

 




