---
description: Функция AMovieDllRegisterServer2 регистрирует и отменяет регистрацию фильтров.
ms.assetid: 2122949d-0117-4c68-bfcd-c717b14dc970
title: Функция AMovieDllRegisterServer2 (Дллсетуп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- AMovieDllRegisterServer2
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: ec36290b7cad66b2b5f27633d30ae76c3331eba9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162320"
---
# <a name="amoviedllregisterserver2-function"></a>Функция AMovieDllRegisterServer2

Функция **AMovieDllRegisterServer2** регистрирует и отменяет регистрацию фильтров.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT AMovieDllRegisterServer2(
   BOOL bRegister
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*брегистер* 
</dt> <dd>

**Значение true** указывает зарегистрировать фильтр, **значение false** — отменить регистрацию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если эта функция завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Используйте эту функцию для настройки фильтров. дополнительные сведения см. [в статье регистрация DirectShow фильтров](how-to-register-directshow-filters.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>дллсетуп. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Функции установки DLL**](dll-setup-functions.md)
</dt> </dl>

 

 




