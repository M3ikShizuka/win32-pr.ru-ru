---
description: Метод Жеткуррентсампле извлекает текущий образец.
ms.assetid: cfdc66e3-7d32-47b7-87f6-99dd9513c93b
title: Кбасерендерер. Жеткуррентсампле, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.GetCurrentSample
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 48c42ff02b22d30138fcad7d1e8af5e57a391b99
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053581"
---
# <a name="cbaserenderergetcurrentsample-method"></a>Кбасерендерер. Жеткуррентсампле, метод

`GetCurrentSample`Метод извлекает текущий образец.

## <a name="syntax"></a>Синтаксис


```C++
virtual IMediaSample* GetCurrentSample();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на интерфейс [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) образца или **значение NULL** , если образец недоступен.

## <a name="remarks"></a>Комментарии

Если метод не возвращает **значение NULL**, метод вызывает **AddRef** для указателя [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) перед возвращением. Вызывающий объект должен освободить указатель. (Неявно, необходимо присвоить возвращаемое значение переменной, чтобы его можно было освободить позже.)

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




