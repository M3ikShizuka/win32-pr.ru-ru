---
description: Метод IsValid определяет, был ли для этого объекта назначен основной тип.
ms.assetid: 22d28019-f360-4b93-972c-d1dfe83938f0
title: Метод Кмедиатипе. IsValid (Мтипе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaType.IsValid
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 7d8e1731060021b61eb5037e1baeeda95021e8f5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362529"
---
# <a name="cmediatypeisvalid-method"></a>Кмедиатипе. IsValid, метод

`IsValid`Метод определяет, был ли присвоен основной тип этому объекту.

## <a name="syntax"></a>Синтаксис


```C++
BOOL IsValid() const;
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если этому объекту был назначен основной тип. В противном случае возвращает **значение false**.

## <a name="remarks"></a>Комментарии

По умолчанию объекты [**кмедиатипе**](cmediatype.md) инициализируются с помощью основного типа GUID \_ null. Вызовите этот метод, чтобы определить, правильно ли инициализирован объект.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>мтипе. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кмедиатипе**](cmediatype.md)
</dt> </dl>

 

 




