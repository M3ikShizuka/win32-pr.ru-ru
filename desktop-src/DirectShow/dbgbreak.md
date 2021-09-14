---
description: Отображает окно сообщения с указанной строкой, именем исходного файла и номером строки. Пользователь может проигнорировать сообщение, ввести отладчик или выйти из приложения. Игнорируется в розничных сборках.
ms.assetid: ac4da7da-f9d0-44ae-9ad1-9a5908b288fb
title: Макрос Дбгбреак (Вксдебуг. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DbgBreak
api_type:
- HeaderDef
api_location:
- Wxdebug.h
ms.openlocfilehash: 099344a295de2657b40218b993ab9c4cb6411353
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362440"
---
# <a name="dbgbreak-macro"></a>Макрос Дбгбреак

Отображает окно сообщения с указанной строкой, именем исходного файла и номером строки. Пользователь может проигнорировать сообщение, ввести отладчик или выйти из приложения. Игнорируется в розничных сборках.

## <a name="syntax"></a>Синтаксис


```C++
void DbgBreak(
    strLiteral
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*стрлитерал* 
</dt> <dd>

Текстовая строка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот макрос не возвращает значение.

## <a name="examples"></a>Примеры


```C++
DbgBreak("Unrecoverable error occurred.");
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>вксдебуг. h (включает Потоки. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Макросы Assert и точка останова](assert-and-breakpoint-macros.md)
</dt> </dl>

 

 




