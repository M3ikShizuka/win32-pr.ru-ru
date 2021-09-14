---
description: Проверяет, соответствует ли указатель заданной границе. В противном случае этот макрос вызывает макрос ASSERT. Игнорируется в розничных сборках.
ms.assetid: 4d9ec3a9-7107-45a3-a7aa-28d6e38fa92a
title: Макрос Дбгассерталигнед (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DbgAssertAligned
api_type:
- HeaderDef
api_location:
- Wxdebug.h
ms.openlocfilehash: 22b357f7f28e9df04ce36636e3972dbadc3036a6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362445"
---
# <a name="dbgassertaligned-macro"></a>Макрос Дбгассерталигнед

Проверяет, соответствует ли указатель заданной границе. В противном случае этот макрос вызывает макрос [**Assert**](assert.md) . Игнорируется в розничных сборках.

## <a name="syntax"></a>Синтаксис


```C++
void DbgAssertAligned(
    ptr,
    alignment
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*указатель* 
</dt> <dd>

Переменная указателя.

</dd> <dt>

*Выравнивание* 
</dt> <dd>

Требуемое выравнивание.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот макрос не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Макросы Assert и точка останова](assert-and-breakpoint-macros.md)
</dt> </dl>

 

 




