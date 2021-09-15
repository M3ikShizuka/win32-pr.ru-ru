---
description: Метод notify получает уведомление о том, что запрошено изменение качества.
ms.assetid: bb9aa1c3-caef-42fb-87d2-75cc3691f64f
title: Метод Кбасевидеорендерер. notify (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseVideoRenderer.Notify
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: cd2b894bf78163a7b2d2387e43ecb5cec76ffdf4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461960"
---
# <a name="cbasevideorenderernotify-method"></a>Кбасевидеорендерер. notify, метод

`Notify`Метод получает уведомление о том, что запрошено изменение качества.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Notify(
  [in] IBaseFilter *pSelf,
  [in] Quality     q
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пселф* \[ окне\]
</dt> <dd>

Указатель на фильтр, отправляющий уведомление.

</dd> <dt>

*вопросы* \[ в\]
</dt> <dd>

Структура уведомления об изменении качества.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Эта функция члена реализует метод [**икуалитиконтрол:: notify**](/windows/desktop/api/Strmif/nf-strmif-iqualitycontrol-notify) в модуле подготовки видео. Этот метод вызывается, как правило, диспетчером графа фильтров, когда необходимо вырезать качество. Это может произойти, когда качество воспроизведения звука увеличилось до момента, когда необходимо уменьшить качество воспроизведения видео.

`Notify` Задает для элемента данных **m \_ трсроттле** значение задержки, которое должно быть вставлено между кадрами [**сроттлеваит**](cbasevideorenderer-throttlewait.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасевидеорендерер**](cbasevideorenderer.md)
</dt> </dl>

 

 




