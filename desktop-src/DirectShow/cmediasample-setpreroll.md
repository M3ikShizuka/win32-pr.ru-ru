---
description: 'Метод Сетпреролл указывает, является ли этот пример примером предобразца. Образец не должен отображаться. Этот метод реализует метод Имедиасампле:: Сетпреролл.'
ms.assetid: 2887e627-5999-407a-88d3-811c803c9a43
title: Кмедиасампле. Сетпреролл, метод (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaSample.SetPreroll
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 594f26ebb738a986c85a14b88f8896b122b58f47
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127251167"
---
# <a name="cmediasamplesetpreroll-method"></a>Кмедиасампле. Сетпреролл, метод

`SetPreroll`Метод указывает, является ли этот пример примером предобразца. Образец не должен отображаться. Этот метод реализует метод [**имедиасампле:: сетпреролл**](/windows/desktop/api/Strmif/nf-strmif-imediasample-setpreroll) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetPreroll(
   BOOL bIsPreroll
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*биспреролл* 
</dt> <dd>

Логическое значение, указывающее, является ли этот пример примером. Если **значение равно true**, это пример предобразца.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Remarks

Этот метод обновляет переменную члена [**кмедиасампле:: m \_ dwFlags**](cmediasample-m-dwflags.md) , которая указывает свойство "предвращение".

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиасампле**](cmediasample.md)
</dt> </dl>

 

 




