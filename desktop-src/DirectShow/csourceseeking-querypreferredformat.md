---
description: 'Метод Куерипреферредформат извлекает предпочтительный формат времени объекта. Этот метод реализует метод Имедиасикинг:: Куерипреферредформат.'
ms.assetid: 3b73b7cf-1ba7-47c5-8442-5f138b74f335
title: Ксаурцесикинг. Куерипреферредформат, метод (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.QueryPreferredFormat
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 5fb311181adf1e36a8f1e46a467cf801de0dcc6d1caaf09a890eb06e43726d04
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120053944"
---
# <a name="csourceseekingquerypreferredformat-method"></a>Ксаурцесикинг. Куерипреферредформат, метод

`QueryPreferredFormat`Метод получает предпочтительный формат времени объекта. Этот метод реализует метод [**имедиасикинг:: куерипреферредформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-querypreferredformat) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT QueryPreferredFormat(
   GUID *pFormat
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пформат* 
</dt> <dd>

Указатель на переменную, которая получает GUID формата времени. См. раздел [**идентификаторы GUID формата времени**](time-format-guids.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , перечисленных в следующей таблице.



| Код возврата                                                                               | Описание                       |
|-------------------------------------------------------------------------------------------|-----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>      | Success<br/>                |
| <dl> <dt>**\_указатель E**</dt> </dl> | Значение указателя **null**<br/> |



 

## <a name="remarks"></a>Remarks

Единственный формат времени, поддерживаемый базовым классом, — это \_ \_ время носителя формата времени \_ (100-наносекундных единиц).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




