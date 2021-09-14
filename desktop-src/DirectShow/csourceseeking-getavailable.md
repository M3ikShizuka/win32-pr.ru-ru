---
description: 'Метод Ксаурцесикинг. дальнего действия. метод доступа к доступности извлекает диапазон времени, в течение которого поиск является эффективным. Этот метод реализует метод Имедиасикинг:: onavailable.'
ms.assetid: 2a7b6cdb-47c3-4aeb-89ff-ea968c6a809b
title: Метод Ксаурцесикинг. Available (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking.GetAvailable
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: f24bc667eec4f5b21c90415e4721aa8cf0a0ad4c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971606"
---
# <a name="csourceseekinggetavailable-method"></a>Ксаурцесикинг. доступный метод

`GetAvailable`Метод извлекает диапазон времени, в котором поиск является эффективным. Этот метод реализует метод [**имедиасикинг:: onavailable**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-getavailable) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetAvailable(
   LONGLONG *pEarliest,
   LONGLONG *pLatest
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пеарлиест* 
</dt> <dd>

Указатель на переменную, которая получает самое раннее время для эффективного поиска. Переменная имеет значение 0.

</dd> <dt>

*Пластина* 
</dt> <dd>

Указатель на переменную, которая получает Последнее время для эффективного поиска. Переменной присваивается значение переменной-члена [**ксаурцесикинг:: m \_ ртдуратион**](csourceseeking-m-rtduration.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксаурцесикинг**](csourceseeking.md)
</dt> </dl>

 

 




