---
description: Функция Дбгтерминате очищает библиотеку отладки. Игнорируется в розничных сборках.
ms.assetid: a0e23c57-b4b5-4bcf-8c63-0dee40cc71a7
title: Функция Дбгтерминате (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DbgTerminate
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: d29e5fde86b9573261e39a0dbe2e9d87018ff23c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127255265"
---
# <a name="dbgterminate-function"></a>Функция Дбгтерминате

Функция **дбгтерминате** очищает библиотеку отладки. Игнорируется в розничных сборках.

## <a name="syntax"></a>Синтаксис


```C++
void DbgTerminate(void);
```



## <a name="parameters"></a>Параметры

У этой функции нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Комментарии

Вызовите эту функцию, если вызывается функция [**дбгинитиалисе**](dbginitialise.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Выходные функции отладки](debug-output-functions.md)
</dt> </dl>

 

 




