---
title: Функция Глуделетекуадрик (GLU. h)
description: Функция Глуделетекуадрик уничтожает объект куадрик.
ms.assetid: 09efd887-0fe8-4a56-bc6f-2177a4930035
keywords:
- Функция Глуделетекуадрик OpenGL
topic_type:
- apiref
api_name:
- gluDeleteQuadric
api_location:
- glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9b5ee85e943cd958e394efb191932393d228d948
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064951"
---
# <a name="gludeletequadric-function"></a>Функция Глуделетекуадрик

Функция **глуделетекуадрик** уничтожает объект куадрик.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI gluDeleteQuadric(
   GLUquadricObj *state
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*state* 
</dt> <dd>

Объект куадрик для уничтожения (созданный с помощью [**глуневкуадрик**](glunewquadric.md)).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Функция **глуделетекуадрик** уничтожает объект куадрик и освобождает используемую память. После вызова **глуделетекуадрик** *состояние* нельзя использовать снова.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Glu. h</dt> </dl>     |
| Библиотека<br/>                  | <dl> <dt>Glu32. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Glu32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**глуневкуадрик**](glunewquadric.md)
</dt> </dl>

 

 





