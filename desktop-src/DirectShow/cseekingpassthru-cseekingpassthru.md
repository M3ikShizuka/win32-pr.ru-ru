---
description: Метод конструктора Ксикингпасссру. Ксикингпасссру.
ms.assetid: e31253fc-b365-4414-9dee-906d4c41d16e
title: Конструктор Ксикингпасссру. Ксикингпасссру (Сикпт. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSeekingPassThru.CSeekingPassThru
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: cab9d6329f5175c96a3bfc5962ca5a555fe62b5d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058011"
---
# <a name="cseekingpassthrucseekingpassthru-constructor"></a>Ксикингпасссру. Ксикингпасссру, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CSeekingPassThru(
   const TCHAR     *pName,
         LPUNKNOWN pUnk,
         HRESULT   *phr
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pName* 
</dt> <dd>

Строка, содержащая имя объекта. Дополнительные сведения см. в разделе [**кбасеобжект**](cbaseobject.md) .

</dd> <dt>

*pUnk* 
</dt> <dd>

Указатель на владельца этого объекта. Если объект является агрегатным, передайте указатель на интерфейс **IUnknown** объекта агрегирования. В противном случае присвойте этому параметру **значение NULL**.

</dd> <dt>

*фр* 
</dt> <dd>

Указатель на значение **HRESULT** . Не обрабатывается.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>сикпт. h (включает Потоки. h)</dt> </dl>                                                                                    |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Ксикингпасссру**](cseekingpassthru.md)
</dt> </dl>

 

 




