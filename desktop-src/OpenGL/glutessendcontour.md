---
title: Функция Глутессендконтаур (GLU. h)
description: Функции Глутессбегинконтаур и Глутессендконтаур разделяют описание контура. | Функция Глутессендконтаур (GLU. h)
ms.assetid: 115db079-cbcb-48e1-8bab-0eb4814afb82
keywords:
- Функция Глутессендконтаур OpenGL
topic_type:
- apiref
api_name:
- gluTessEndContour
api_location:
- Glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6ac53f3920476489a1453bb6b5dc1e01d650d4fe
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064927"
---
# <a name="glutessendcontour-function"></a>Функция Глутессендконтаур

Функции [**глутессбегинконтаур**](glutessbegincontour.md) и **глутессендконтаур** разделяют описание контура.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI gluTessEndContour(
   GLUtesselator *tess
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тесс* 
</dt> <dd>

Объект тесселяции (созданный с помощью [**глуневтесс**](glunewtess.md)).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Функции [**глутессбегинконтаур**](glutessbegincontour.md) и **глутессендконтаур** разделяют определение контура многоугольника. Внутри каждой пары **глутессбегинконтаур** / **глутессендконтаур** может быть несколько вызовов [**глутессвертекс**](glutessvertex.md). Вершины задают замкнутый контур (последняя вершина каждого контура автоматически связывается с первым). **Глутессбегинконтаур** можно вызывать только между [**глутессбегинполигон**](glutessbeginpolygon.md) и [**глутессендполигон**](glutessendpolygon.md).

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

[**глуневтесс**](glunewtess.md)
</dt> <dt>

[**глутессбегинполигон**](glutessbeginpolygon.md)
</dt> <dt>

[*глутесскаллбакк*](glutess.md)
</dt> <dt>

[**глутессендполигон**](glutessendpolygon.md)
</dt> <dt>

[**глутесснормал**](glutessnormal.md)
</dt> <dt>

[**глутесспроперти**](glutessproperty.md)
</dt> <dt>

[**глутессвертекс**](glutessvertex.md)
</dt> </dl>

 

 





