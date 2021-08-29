---
description: Метод Run запускает фильтр.
ms.assetid: 83251137-83f8-45a3-b3f2-d7b45f43f7f8
title: Метод Кбасерендерер. Run (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.Run
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4c07c89354d1885fcc70799b3aaf4cc651668bda80ddadd30dbe74c77a2b6275
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119999694"
---
# <a name="cbaserendererrun-method"></a>Кбасерендерер. Run, метод

`Run`Метод выполняет фильтр.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Run();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК в случае успешного выполнения или **HRESULT** , указывающий на причину ошибки.

## <a name="remarks"></a>Remarks

Этот метод переопределяет метод [**кбасефилтер:: Run**](cbasefilter-run.md) . Он выполняет следующие действия:

-   Вызывает метод **кбасефилтер:: Run** .
-   Фиксирует распределитель. (См. [**имемаллокатор:: Commit**](/windows/desktop/api/Strmif/nf-strmif-imemallocator-commit).)
-   Если предыдущее состояние было остановлено, фильтр выпустит любой пример, который он удерживает. (Образец больше не является допустимым.)
-   Вызывает метод [**кбасерендерер:: стартстреаминг**](cbaserenderer-startstreaming.md) и возвращает результат. Если пример находится в состоянии ожидания, метод **стартстреаминг** планирует его для подготовки к просмотру.

Если фильтр не подключен, он сразу же отправляет событие [**EC \_ Complete**](ec-complete.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




