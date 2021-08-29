---
title: Функция Глуневтесс (GLU. h)
description: Функция Глуневтесс создает объект тесселяции.
ms.assetid: dfc9fce8-ecab-493b-85ee-6d7487814186
keywords:
- Функция Глуневтесс OpenGL
topic_type:
- apiref
api_name:
- gluNewTess
api_location:
- glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2bc0d11b18425431eadca22f3c541eecf0f3c194b8c6ce897932c33d1674b179
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119519584"
---
# <a name="glunewtess-function"></a>Функция Глуневтесс

Функция **глуневтесс** создает объект тесселяции.

## <a name="syntax"></a>Синтаксис


```C++
GLUtesselator* WINAPI gluNewTess(void);
```



## <a name="parameters"></a>Параметры

У этой функции нет параметров.

## <a name="remarks"></a>Remarks

Функция **глуневтесс** создает и возвращает указатель на новый объект тесселяции. Используйте этот объект при вызове функций тесселяции. Возвращаемое значение, равное нулю, означает, что недостаточно памяти для выделения объекту.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Glu. h</dt> </dl>     |
| Библиотека<br/>                  | <dl> <dt>Glu32. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Glu32.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**глуделететесс**](gludeletetess.md)
</dt> <dt>

[**глутессбегинполигон**](glubeginpolygon.md)
</dt> <dt>

[*глутесскаллбакк*](glutess.md)
</dt> </dl>

 

 





