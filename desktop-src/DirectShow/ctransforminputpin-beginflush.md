---
description: 'Метод Бегинфлуш начинает операцию очистки. Этот метод реализует метод Ипин:: Бегинфлуш.'
ms.assetid: 7c76ca06-dc3c-4f9a-9761-32aea7db4c7e
title: Ктрансформинпутпин. Бегинфлуш, метод (Трансфрм. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CTransformInputPin.BeginFlush
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a4d028634364ca59ae293d9ebb60a464974ccd74
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246631"
---
# <a name="ctransforminputpinbeginflush-method"></a>Ктрансформинпутпин. Бегинфлуш, метод

`BeginFlush`Метод начинает операцию записи на диск. Этот метод реализует метод [**Ипин:: бегинфлуш**](/windows/desktop/api/Strmif/nf-strmif-ipin-beginflush) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT BeginFlush();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Возможные значения включают в себя, показанные в следующей таблице.



| Код возврата                                                                                           | Описание                             |
|-------------------------------------------------------------------------------------------------------|-----------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>                  | Успешно.<br/>                     |
| <dl> <dt>**VFW \_ E \_ не \_ подключен**</dt> </dl> | Выходной ПИН-код не подключен.<br/> |



 

## <a name="remarks"></a>Remarks

Этот метод вызывает метод [**кбасеинпутпин:: бегинфлуш**](cbaseinputpin-beginflush.md) ПИН-кода. Затем вызывается метод [**ктрансформфилтер:: бегинфлуш**](ctransformfilter-beginflush.md) фильтра для предоставления вызова в нисходящем направлении.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>трансфрм. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




