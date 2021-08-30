---
description: Метод ClassID определяет, соответствует ли CLSID этому шаблону класса.
ms.assetid: de560f7a-2ccb-44e2-ac32-3b0fea0d80b8
title: Метод Кфакторитемплате. ClassID (Комбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CFactoryTemplate.IsClassID
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 38714c6c6a97c46a14d1e381fdf49ddbc723d04ee217a09c9554b39d4eb22491
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120055794"
---
# <a name="cfactorytemplateisclassid-method"></a>Кфакторитемплате. ClassID, метод

`IsClassID`Метод определяет, соответствует ли CLSID этому шаблону класса.

## <a name="syntax"></a>Синтаксис


```C++
BOOL IsClassID(
   REFCLSID rclsid
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*рклсид* 
</dt> <dd>

Ссылка на идентификатор CLSID.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если параметр *рклсид* является тем же идентификатором CLSID, что и переменная-член [**\_ кфакторитемплате:: m**](cfactorytemplate-m-clsid.md) , или Else возвращает **значение false**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кфакторитемплате**](cfactorytemplate.md)
</dt> </dl>

 

 




