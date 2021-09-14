---
description: Флаг, указывающий, пытается ли ПИН-код использовать собственные предпочтительные типы мультимедиа перед приемом ПИН-кода.
ms.assetid: 50462ee4-4a61-472f-9a7e-9cdb39be4dea
title: 'Элемент Кбасепин:: m_bTryMyTypesFirst (Амфилтер. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- m_bTryMyTypesFirst
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 72f98021b6ba97d32974f26ac4e76ca31fa54e5c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971861"
---
# <a name="cbasepinm_btrymytypesfirst-member"></a>Элемент Кбасепин:: m \_ бтримитипесфирст

Флаг, указывающий, пытается ли ПИН-код использовать собственные предпочтительные типы мультимедиа перед приемом ПИН-кода.

## <a name="syntax"></a>Синтаксис


```C++
bool m_bTryMyTypesFirst;
```



## <a name="remarks"></a>Remarks

По умолчанию этот флаг **имеет значение false**. Если флаг имеет **значение true**, метод [**Кбасепин:: агримедиатипе**](cbasepin-agreemediatype.md) меняет порядок, в котором он пытается выполнить типы мультимедиа.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасепин**](cbasepin.md)
</dt> </dl>

 

 




