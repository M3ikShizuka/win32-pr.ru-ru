---
description: Метод конструктора Кункновн. Кункновн.
ms.assetid: dafe0d5c-b4c8-4efb-8c47-a8c5db6e8aed
title: Конструктор Кункновн. Кункновн (Комбасе. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CUnknown.CUnknown
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 32859871f8ef69ce357fe204f0741356314fbb06
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255271"
---
# <a name="cunknowncunknown-constructor"></a>Кункновн. Кункновн, конструктор

Метод конструктора.

## <a name="syntax"></a>Синтаксис


```C++
CUnknown(
   const TCHAR     *pName,
         LPUNKNOWN pUnk
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pName* 
</dt> <dd>

Строка, содержащая имя объекта; используется в конструкторе [**кбасеобжект**](cbaseobject.md) для отладки.

</dd> <dt>

*pUnk* 
</dt> <dd>

Указатель на владельца этого объекта. Если объект является агрегатным, передайте указатель на интерфейс IUnknown объекта агрегирования. В противном случае присвойте этому параметру **значение NULL**.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Объект инициализируется с нулевым значением счетчика ссылок.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>комбасе. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




