---
description: Проверяет, имеет ли вызывающий процесс доступ на чтение к строке. В противном случае макрос вызывает макрос Дбгбреак.
ms.assetid: 749a8c22-7a4a-49c2-a214-fc64dc5a0202
title: Макрос Валидатестрингптр (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ValidateReadPtr
api_type:
- HeaderDef
api_location:
- Wxdebug.h
ms.openlocfilehash: 19bf0b9e43ecbbbdea0e11284cd1cb4a058e22cc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169888"
---
# <a name="validatestringptr-macro"></a>Макрос Валидатестрингптр

Проверяет, имеет ли вызывающий процесс доступ на чтение к строке. В противном случае макрос вызывает макрос [**дбгбреак**](dbgbreak.md) .

> [!Note]  
> Этот макрос не рекомендуется к использованию. в Windows SDK для Windows Vista (и более поздних версий) этот макрос не выполняет никаких действий.

 

## <a name="syntax"></a>Синтаксис


```C++
void ValidateReadPtr(
   LPCTSTR p
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ш* 
</dt> <dd>

Указатель на строку **TCHAR** , заканчивающуюся нулем.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот макрос не возвращает значение.

## <a name="remarks"></a>Remarks

этот макрос игнорируется, если \_ при включении файла заголовка DirectShow базового класса не определена отладка, отладка или вфвробуст. Этот макрос может существенно постоить в производительности.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Макросы проверки указателя](pointer-validation-macros.md)
</dt> </dl>

 

 




