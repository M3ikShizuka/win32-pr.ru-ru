---
title: Функция Глуендсурфаце (GLU. h)
description: Функции Глубегинсурфаце и Глуендсурфаце разделяют неоднородное рациональное определение поверхности B-сплайна (НУРБС). | Функция Глуендсурфаце (GLU. h)
ms.assetid: beaa0340-c67d-4376-bedd-7f73c5c6d742
keywords:
- Функция Глуендсурфаце OpenGL
topic_type:
- apiref
api_name:
- gluEndSurface
api_location:
- Glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 54631d5c4ef752cffd989f8fa02f8cb512c67da3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064939"
---
# <a name="gluendsurface-function"></a>Функция Глуендсурфаце

Функции [**глубегинсурфаце**](glubeginsurface.md) и **глуендсурфаце** разделяют неоднородное рациональное определение поверхности B-сплайна ([нурбс](using-nurbs-curves-and-surfaces.md)).

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI gluEndSurface(
   GLUnurbs *nobj
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*нобж* 
</dt> <dd>

Объект НУРБС (созданный с помощью [**глуневнурбсрендерер**](glunewnurbsrenderer.md)).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Функции [**глубегинсурфаце**](glubeginsurface.md) и **глуендсурфаце** отмечают начало и конец определений нурбс Surface, которые определяются вызовами **глунурбссурфаце**.

1.  Вызовите **глубегинсурфаце** , чтобы пометить начало определения поверхности нурбс.
2.  Выполните один или несколько вызовов **глунурбссурфаце** , чтобы определить атрибуты поверхности.

    Ровно один из этих вызовов **глунурбссурфаце** должен иметь тип поверхности GL \_ MAP2 \_ Vertex \_ 3 или GL \_ MAP2 \_ Vertex \_ 4.

3.  Чтобы отметить конец определения поверхности НУРБС, вызовите **глуендсурфаце**.

Функции [**глубегинтрим**](glubegintrim.md), [**глупвлкурве**](glupwlcurve.md), [**глунурбскурве**](glunurbscurve.md)и **глуендтрим** поддерживают усечение поверхностей нурбс.

Используйте оценщики OpenGL для отрисовки поверхности НУРБС в виде набора многоугольников. Сохраните состояние оценщика во время подготовки к просмотру с помощью [**глпушаттриб**](glpushattrib.md) ( \_ бит главной оценки \_ ) и [**глпопаттриб**](glpopattrib.md).

## <a name="examples"></a>Примеры

Следующие функции отрисовывают текстурную поверхность НУРБС с нормальными, координаты текстуры и нормали также описаны как НУРБСные поверхности:

``` syntax
gluBeginSurface(nobj); 
    gluNurbsSurface(nobj, . . ., GL_MAP2_TEXTURE_COORD_2); 
    gluNurbsSurface(nobj, . . ., GL_MAP2_NORMAL); 
    gluNurbsSurface(nobj, . . ., GL_MAP2_VERTEX_4); 
gluEndSurface(nobj);
```

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

[**глубегинкурве**](glubegincurve.md)
</dt> <dt>

[**глубегинтрим**](glubegintrim.md)
</dt> <dt>

[**глуневнурбсрендерер**](glunewnurbsrenderer.md)
</dt> <dt>

[**глунурбскурве**](glunurbscurve.md)
</dt> <dt>

[**глунурбссурфаце**](glunurbssurface.md)
</dt> <dt>

[**глупвлкурве**](glupwlcurve.md)
</dt> </dl>

 

 





