---
description: Указатель функции Лпфнневкомобжект — указатель на функцию, которая создает экземпляр объекта.
ms.assetid: 8c9dab82-a080-4733-8c62-d090b28306e0
title: Указатель функции Лпфнневкомобжект (Комбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- LPFNNewCOMObject
api_type:
- UserDefined
api_location:
- Combase.h
ms.openlocfilehash: f3ea5bc172bc22f7aa9dce1f348bba552520565f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055439"
---
# <a name="lpfnnewcomobject-function-pointer"></a>Указатель функции Лпфнневкомобжект

Указатель на функцию, которая создает экземпляр объекта.

## <a name="syntax"></a>Синтаксис


```C++
typedef CUnknown* ( CALLBACK *LPFNNewCOMObject)(
   LPUNKNOWN pUnkOuter,
   HRESULT   *phr
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пункаутер* 
</dt> <dd>

Указатель на интерфейс **IUnknown** объекта, который выполняет статистическую обработку нового объекта, если он имеется. Этот указатель может иметь **значение NULL**.

</dd> <dt>

*фр* 
</dt> <dd>

Указатель на значение **HRESULT** . Если конструктор завершается неудачно, этот параметр получает код ошибки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает указатель на новый экземпляр объекта.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Кфакторитемплате**](cfactorytemplate.md)
</dt> </dl>

 

 




