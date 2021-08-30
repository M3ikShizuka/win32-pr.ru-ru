---
description: Метод размещения \_ баккграундпалетте устанавливает флаг для реализации палитры в фоновом режиме.
ms.assetid: db420e75-e300-41fa-bae4-fb267cc99c7c
title: Метод CBaseControlWindow.put_BackgroundPalette (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseControlWindow.put_BackgroundPalette
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 295889510b96a085865eeff45ba976278519670adbd596b24e6aea829a29df4e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119966723"
---
# <a name="cbasecontrolwindowput_backgroundpalette-method"></a>Кбасеконтролвиндов. размещение \_ метода баккграундпалетте

`put_BackgroundPalette`Метод задает флаг для реализации палитры в фоновом режиме.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_BackgroundPalette(
   long BackgroundPalette
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*баккграундпалетте* 
</dt> <dd>

Логический флаг автоматизации (0 — отключено, 1 — включено).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** .

## <a name="remarks"></a>Remarks

Для воспроизведения видео в другом приложении или документе может потребоваться использовать собственную палитру. Он может задать, чтобы видео использовало текущую палитру переднего плана, а не собственную в качестве палитры фона, установив для этого флага значение 1. Если задано значение 0, окно будет установлено и использовать собственную предпочтительную палитру. Запрос использования другой палитры в окне приведет к значительному снижению производительности.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасеконтролвиндов**](cbasecontrolwindow.md)
</dt> </dl>

 

 




