---
description: Проверяет, имеет ли вызывающий процесс доступ на чтение к строке расширенных символов. В противном случае макрос вызывает макрос Дбгбреак.
ms.assetid: 526e8027-31e5-428d-856d-9fc6698693c3
title: Макрос Валидатестрингптрв (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ValidateStringPtrW
api_type:
- HeaderDef
api_location:
- Wxdebug.h
ms.openlocfilehash: 1ece2caa0f2263c038121cd1ffd031cbe42d336a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169880"
---
# <a name="validatestringptrw-macro"></a>Макрос Валидатестрингптрв

Проверяет, имеет ли вызывающий процесс доступ на чтение к строке расширенных символов. В противном случае макрос вызывает макрос [**дбгбреак**](dbgbreak.md) .

> [!Note]  
> Этот макрос не рекомендуется к использованию. в Windows SDK для Windows Vista (и более поздних версий) этот макрос не выполняет никаких действий.

 

## <a name="syntax"></a>Синтаксис


```C++
void ValidateStringPtrW(
   LPCWSTR p
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ш* 
</dt> <dd>

Указатель на строку расширенных символов, заканчивающуюся НУЛЕМ.

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

 

 




