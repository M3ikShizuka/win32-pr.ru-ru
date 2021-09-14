---
description: Метод INSERT добавляет объект Кдеферредкомманд в очередь.
ms.assetid: 41f9c30c-6267-435a-9089-eb34ae606896
title: Метод Ккмдкуеуе. Insert (Винутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CCmdQueue.Insert
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 6bad004641258e29ed42d7142a5b0ab2c0ceb78d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147865"
---
# <a name="ccmdqueueinsert-method"></a>Ккмдкуеуе. INSERT, метод

`Insert`Метод добавляет объект [**кдеферредкомманд**](cdeferredcommand.md) в очередь.

## <a name="syntax"></a>Синтаксис


```C++
virtual HRESULT Insert(
   CDeferredCommand *pCmd
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pCmd* 
</dt> <dd>

Указатель на объект **кдеферредкомманд** для добавления в очередь.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ ОК в реализации по умолчанию.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>винутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ккмдкуеуе**](ccmdqueue.md)
</dt> </dl>

 

 




