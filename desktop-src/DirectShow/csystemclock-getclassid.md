---
description: Метод WebMethod извлекает идентификатор класса (CLSID) объекта. Этот метод реализует метод IPersist::/ClassID.
ms.assetid: 3d2cc6a3-67d1-4dd9-916b-7c350ce6a542
title: Метод Ксистемклокк. ClassID (Сисклокк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSystemClock.GetClassID
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: a2f83d3e3c2efcbcb5d4604bc5c50a37dc020f0a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057972"
---
# <a name="csystemclockgetclassid-method"></a>Ксистемклокк. ClassID, метод

`GetClassID`Метод получает идентификатор класса (CLSID) объекта. Этот метод реализует метод **IPersist::/ClassID** .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetClassID(
   CLSID *pClsID
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пклсид* 
</dt> <dd>

Указатель на переменную, которая получает значение CLSID \_ системклокк.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение S \_ (ОК) или \_ указатель E.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Класс Ксистемклокк<br/>                                                                                                                                                              |
| Заголовок<br/>  | <dl> <dt>сисклокк. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




