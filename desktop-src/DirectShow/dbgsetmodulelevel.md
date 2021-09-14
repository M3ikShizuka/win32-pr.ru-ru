---
description: Функция Дбгсетмодулелевел задает уровень ведения журнала для одного или нескольких типов сообщений. Игнорируется в розничных сборках.
ms.assetid: 89d25106-8018-4089-8b77-d3c87529e984
title: Функция Дбгсетмодулелевел (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DbgSetModuleLevel
api_type:
- LibDef
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 1d6623793b150c600eb00f0c0843dd72c68deb4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054621"
---
# <a name="dbgsetmodulelevel-function"></a>Функция Дбгсетмодулелевел

Функция **дбгсетмодулелевел** задает уровень ведения журнала для одного или нескольких типов сообщений. Игнорируется в розничных сборках.

## <a name="syntax"></a>Синтаксис


```C++
void DbgSetModuleLevel(
   DWORD Types,
   DWORD Level
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Типы* 
</dt> <dd>

Побитовое сочетание одного или нескольких типов сообщений.

</dd> <dt>

*Уровень* 
</dt> <dd>

Уровень ведения журнала для указанных типов сообщений.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Выходные функции отладки](debug-output-functions.md)
</dt> </dl>

 

 




