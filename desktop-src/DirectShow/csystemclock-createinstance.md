---
description: Метод CreateInstance создает новый экземпляр этого объекта.
ms.assetid: 5c62f781-0f22-4d8f-8517-272405dd07c5
title: Метод Ксистемклокк. CreateInstance (Сисклокк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSystemClock.CreateInstance
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 264997448aea028c5725d207ce4b301d369a092c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057968"
---
# <a name="csystemclockcreateinstance-method"></a>Ксистемклокк. CreateInstance, метод

`CreateInstance`Метод создает новый экземпляр этого объекта.

## <a name="syntax"></a>Синтаксис


```C++
static CUnknown* WINAPI CreateInstance(
   LPUNKNOWN pUnk,
   HRESULT   *phr
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pUnk* 
</dt> <dd>

Указатель на агрегированный интерфейс **IUnknown** .

</dd> <dt>

*фр* 
</dt> <dd>

Указатель на переменную, которая получает значение **HRESULT** , указывающее на успешное выполнение или ошибку метода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на новый экземпляр этого объекта.

## <a name="remarks"></a>Remarks

Фабрика классов вызывает этот метод для создания объекта.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>сисклокк. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




