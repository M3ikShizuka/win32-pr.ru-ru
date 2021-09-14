---
description: Метод Register добавляет фильтр в реестр.
ms.assetid: 934e421a-25a6-40fa-a48b-6d7331f34b78
title: Метод Кбасефилтер. Register (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseFilter.Register
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 1bd7ba5a57d670ef28ffda022c95c7dc5b12df77
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347058"
---
# <a name="cbasefilterregister-method"></a>Кбасефилтер. Register, метод

`Register`Метод добавляет фильтр в реестр.

> [!Note]  
> Этот метод устарел. Новые фильтры должны быть зарегистрированы с помощью функции [**AMovieDllRegisterServer2**](amoviedllregisterserver2.md) . дополнительные сведения см. [в статье регистрация DirectShow фильтров](how-to-register-directshow-filters.md).

 

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Register();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений **HRESULT** , перечисленных в следующей таблице.



| Код возврата                                                                             | Описание                                          |
|-----------------------------------------------------------------------------------------|------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>    | Успешно.<br/>                                  |
| <dl> <dt>**S \_ false**</dt> </dl> | Сведения о регистрации недоступны.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кбасефилтер**](cbasefilter.md)
</dt> </dl>

 

 




