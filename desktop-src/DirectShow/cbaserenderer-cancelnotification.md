---
description: Метод Канцелнотификатион отменяет событие таймера, которое планирует подготовку к просмотру.
ms.assetid: 56ddf692-a2e3-40f2-848f-2d592601ec00
title: Кбасерендерер. Канцелнотификатион, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.CancelNotification
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: be7366e6e22aa7e984fe4b50ea29edfa840d78380373d521c6cd8bfd226e1a42
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119635174"
---
# <a name="cbaserenderercancelnotification-method"></a>Кбасерендерер. Канцелнотификатион, метод

`CancelNotification`Метод отменяет событие таймера, которое планирует подготовку к просмотру.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT CancelNotification();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , приведенных в следующей таблице.



| Код возврата                                                                             | Описание                                  |
|-----------------------------------------------------------------------------------------|----------------------------------------------|
| <dl> <dt>**S \_ false**</dt> </dl> | Нет ожидающего события таймера.<br/> |
| <dl> <dt>**\_ОК**</dt> </dl>    | Успешно.<br/>                          |



 

## <a name="remarks"></a>Remarks

Фильтр вызывает этот метод при остановке потоковой передачи. Метод отменяет любую запланированную отрисовку.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




