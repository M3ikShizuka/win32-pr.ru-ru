---
title: Функция Глуделетенурбсрендерер (GLU. h)
description: Функция Глуделетенурбсрендерер уничтожает неравномерный рациональный объект B-сплайна (НУРБС).
ms.assetid: 77063dcb-90b8-47e4-8b00-e1c46cf4f712
keywords:
- Функция Глуделетенурбсрендерер OpenGL
topic_type:
- apiref
api_name:
- gluDeleteNurbsRenderer
api_location:
- glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3fb6ecf0bbb7076d4d6292676d3d358586d0986c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064952"
---
# <a name="gludeletenurbsrenderer-function"></a>Функция Глуделетенурбсрендерер

Функция **глуделетенурбсрендерер** уничтожает неравномерный рациональный объект B-сплайна ([нурбс](using-nurbs-curves-and-surfaces.md)).

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI gluDeleteNurbsRenderer(
   GLUnurbs *nobj
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*нобж* 
</dt> <dd>

Объект НУРБС для уничтожения (созданный с помощью **глуневнурбсрендерер**).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Функция **глуделетенурбсрендерер** уничтожает объект нурбс и освобождает используемую память. После вызова **глуделетенурбсрендерер** нельзя использовать *нобж* повторно.

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

[**глуневнурбсрендерер**](glunewnurbsrenderer.md)
</dt> </dl>

 

 





