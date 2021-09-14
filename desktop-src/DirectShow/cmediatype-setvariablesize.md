---
description: Метод Сетвариаблесизе указывает, что выборки не имеют фиксированного размера.
ms.assetid: 2a207cdb-f8e6-44aa-8bf6-868267aeb42d
title: Кмедиатипе. Сетвариаблесизе, метод (Мтипе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaType.SetVariableSize
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4621a639b3bc18382bc41ae9425c4de50db920ff
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246814"
---
# <a name="cmediatypesetvariablesize-method"></a>Кмедиатипе. Сетвариаблесизе, метод

`SetVariableSize`Метод указывает, что выборки не имеют фиксированного размера.

## <a name="syntax"></a>Синтаксис


```C++
void SetVariableSize();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод задает для элемента **Бфикседсизесамплес** **значение false**. Последующие вызовы метода [**кмедиатипе:: жетсамплесизе**](cmediatype-getsamplesize.md) возвращают ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>мтипе. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиатипе**](cmediatype.md)
</dt> </dl>

 

 




