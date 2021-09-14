---
description: 'Метод EndOfStream уведомляет ПИН-код о том, что дополнительные данные не ожидаются, пока для фильтра не будет выдана новая команда Run. Этот метод реализует метод Ипин:: EndOfStream.'
ms.assetid: 915beab4-2fc3-4acd-bb30-c0851df058db
title: Крендерединпутпин. EndOfStream, метод (Амекстра. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CRenderedInputPin.EndOfStream
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: c836b1098c92a69fa720fb7b87e4a63b3c05a526
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246682"
---
# <a name="crenderedinputpinendofstream-method"></a>Крендерединпутпин. EndOfStream, метод

`EndOfStream`Метод уведомляет ПИН-код о том, что дополнительные данные не ожидаются, пока не будет выполнена новая команда запуска для фильтра. Этот метод реализует метод [**Ипин:: EndOfStream**](/windows/desktop/api/Strmif/nf-strmif-ipin-endofstream) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT EndOfStream();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ ОК, если успешно, или код ошибки в противном случае.

## <a name="remarks"></a>Remarks

если фильтр выполняется, этот метод отправляет событие [**\_ завершения EC**](ec-complete.md) в фильтр Graph Manager. В противном случае устанавливает флаг, чтобы \_ при следующем запуске фильтра было отправлено событие EC Complete. При сбросе фильтра снимается флажок.

Этот метод следует переопределить для удержания потоковой блокировки ПИН-кода:


```C++
class CMyInputPin : public CRenderedInputPin
{
private:
    CCritSec * const m_pReceiveLock; // Streaming lock.
public:
    STDMETHODIMP EndOfStream(void);

    /* (Remainder of the class declaration not shown.) */
};

STDMETHODIMP CMyInputPin::EndOfStream(void)
{
    CAutoLock lock(m_pReceiveLock);  
    return CRenderedInputPin::EndOfStream();
} 
```



Кроме того, если фильтр обрабатывает вызовы **Receive** асинхронно, ПИН-код должен подождать отправки события EC \_ Complete до тех пор, пока фильтр не обработал все отложенные выборки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амекстра. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Крендерединпутпин**](crenderedinputpin.md)
</dt> </dl>

 

 




