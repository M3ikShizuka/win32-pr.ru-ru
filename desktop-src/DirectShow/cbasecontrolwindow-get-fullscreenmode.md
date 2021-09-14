---
description: Метод Get \_ фуллскринмоде извлекает текущий полноэкранный режим.
ms.assetid: 351af361-5cfd-4e82-bd8a-92f629bd270d
title: Метод CBaseControlWindow.get_FullScreenMode (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.get_FullScreenMode
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: fc77b43db2bb420e6cfe2eace44e96e1ab43b0cb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971977"
---
# <a name="cbasecontrolwindowget_fullscreenmode-method"></a>Кбасеконтролвиндов. Get \_ фуллскринмоде, метод

`get_FullScreenMode`Метод извлекает текущий полноэкранный режим.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_FullScreenMode(
   long *FullScreenMode
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*фуллскринмоде* 
</dt> <dd>

Указатель на текущий полноэкранный режим.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Комментарии

Эта функция – член \_ по умолчанию возвращает E нотимпл. Это информирует распространитель подключаемого модуля [**ивидеовиндов**](/windows/desktop/api/Control/nn-control-ivideowindow) о том, что этот модуль подготовки отчетов не реализует полноэкранный визуализатор.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




