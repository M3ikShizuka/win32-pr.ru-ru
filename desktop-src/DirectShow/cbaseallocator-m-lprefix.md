---
description: Префикс каждого буфера в байтах.
ms.assetid: 471b73bf-f959-41aa-84ba-324a2738dd0e
title: 'Элемент Кбасеаллокатор:: m_lPrefix (Амфилтер. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_lPrefix
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fc52db44dcdfa050cf8bc7faf57cb7094d8cac91
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058108"
---
# <a name="cbaseallocatorm_lprefix-member"></a>Элемент Кбасеаллокатор:: m \_ лпрефикс

Префикс каждого буфера в байтах. Если значение не равно нулю, то каждый указатель буфера, возвращенный методом [**кбасеаллокатор::**](cbaseallocator-getbuffer.md) GetBytes, предшествует блоку байтов размером *m \_ лпрефикс*. Этот блок памяти называется *префиксом*. Переменная члена [**кбасеаллокатор:: m \_ лсизе**](cbaseallocator-m-lsize.md) не включает значение префикса.

## <a name="syntax"></a>Синтаксис


```C++
long m_lPrefix;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеаллокатор**](cbaseallocator.md)
</dt> </dl>

 

 




