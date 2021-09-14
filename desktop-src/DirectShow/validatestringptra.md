---
description: Проверяет, имеет ли вызывающий процесс доступ на чтение к строке ANSI. В противном случае макрос вызывает макрос Дбгбреак.
ms.assetid: 44be67f8-9896-4360-82de-083a5f28a3d0
title: Макрос Валидатестрингптра (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ValidateStringPtrA
api_type:
- HeaderDef
api_location:
- Wxdebug.h
ms.openlocfilehash: 94ce34393ec494f34cce621afc168a4d6bbe4325
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169887"
---
# <a name="validatestringptra-macro"></a>Макрос Валидатестрингптра

Проверяет, имеет ли вызывающий процесс доступ на чтение к строке ANSI. В противном случае макрос вызывает макрос [**дбгбреак**](dbgbreak.md) .

> [!Note]  
> Этот макрос не рекомендуется к использованию. в Windows SDK для Windows Vista (и более поздних версий) этот макрос не выполняет никаких действий.

 

## <a name="syntax"></a>Синтаксис


```C++
void ValidateStringPtrA(
   LPCSTR p
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ш* 
</dt> <dd>

Указатель на строку ANSI, заканчивающуюся нулем.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот макрос не возвращает значение.

## <a name="remarks"></a>Remarks

этот макрос игнорируется, если \_ при включении файла заголовка DirectShow базового класса не определена отладка, отладка или вфвробуст.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Макросы проверки указателя](pointer-validation-macros.md)
</dt> </dl>

 

 




