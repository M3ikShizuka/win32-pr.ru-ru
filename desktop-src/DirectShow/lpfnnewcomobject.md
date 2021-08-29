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
ms.openlocfilehash: f589404cd2a4bf5ff42b331cdf48a978d97e9a274a5fc01a483c804f5878b3eb
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119501954"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Класс Кфакторитемплате**](cfactorytemplate.md)
</dt> </dl>

 

 




