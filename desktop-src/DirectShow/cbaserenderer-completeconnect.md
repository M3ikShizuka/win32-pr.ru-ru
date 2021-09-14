---
description: Метод Комплетеконнект завершает подключение входного контакта к другому ПИН-коду.
ms.assetid: 8dfc1a50-bc73-436a-a471-d8d3218410d3
title: Кбасерендерер. Комплетеконнект, метод (Ренбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseRenderer.CompleteConnect
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a9d2d35f99a3b3b8dc5b668b8ee9a9f94f0a53dd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147933"
---
# <a name="cbaserenderercompleteconnect-method"></a>Кбасерендерер. Комплетеконнект, метод

`CompleteConnect`Метод завершает подключение входного контакта к другому ПИН-коду.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT CompleteConnect(
   IPin *pReceivePin
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*прецеивепин* 
</dt> <dd>

Указатель на интерфейс [**Ипин**](/windows/desktop/api/Strmif/nn-strmif-ipin) выходного контакта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ ОК.

## <a name="remarks"></a>Remarks

Входной ПИН-код фильтра вызывает этот метод из собственного `CompleteConnect` метода, который вызывается для завершения соединения с ПИН-кодом. (Дополнительные сведения см. в разделе [**кбасепин:: комплетеконнект**](cbasepin-completeconnect.md).) Фильтр вызывает метод [**кбасерендерер:: сетрепаинтстатус**](cbaserenderer-setrepaintstatus.md) , чтобы включить события [**\_ перерисовки EC**](ec-repaint.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ренбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасерендерер**](cbaserenderer.md)
</dt> </dl>

 

 




