---
title: ID2D1RenderTarget Дравбитмап методы
description: Рисует указанный ID2D1Bitmap.
ms.assetid: 241df698-ca5e-4d94-902a-a9e140820c14
keywords:
- Методы Дравбитмап Direct2D
topic_type:
- apiref
api_location:
- D2d1.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
api_name: ''
ms.openlocfilehash: 46c4e163ebb7c5c17db743687fded2c0f32771a37c0fb4dfa8af9ce45ee2fb86
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119874354"
---
# <a name="id2d1rendertargetdrawbitmap-methods"></a>ID2D1RenderTarget: методы:D Равбитмап

Рисует указанный [**ID2D1Bitmap**](/windows/win32/api/d2d1/nn-d2d1-id2d1bitmap).

### <a name="overload-list"></a>Список перегрузок



| Метод                                                                                                                                                                                                                       | Описание                                                                                     |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------|
| [**Дравбитмап (ID2D1Bitmap \* , D2D1 \_ rect \_ f&, float, D2D1 \_ битовый \_ Режим интерполяции \_ , D2D1 \_ Rect \_ F&)**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-drawbitmap(id2d1bitmap_constd2d1_rect_f__float_d2d1_bitmap_interpolation_mode_constd2d1_rect_f_))   | Рисует заданное растровое изображение после его масштабирования до размера указанного прямоугольника. <br/> |
| [**Дравбитмап (ID2D1Bitmap \* , D2D1 \_ RECT \_ f&, float, D2D1 \_ битовый \_ Режим интерполяции \_ , D2D1 \_ Rect \_ F \* )**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-drawbitmap(id2d1bitmap_constd2d1_rect_f__float_d2d1_bitmap_interpolation_mode_constd2d1_rect_f))  | Рисует заданное растровое изображение после его масштабирования до размера указанного прямоугольника. <br/> |
| [**Дравбитмап (ID2D1Bitmap \* , D2D1 \_ Rect \_ f \* , float, D2D1 \_ БИТОВЫЙ \_ Режим интерполяции \_ , D2D1 \_ Rect \_ F \* )**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-drawbitmap(id2d1bitmap_constd2d1_rect_f_float_d2d1_bitmap_interpolation_mode_constd2d1_rect_f)) | Рисует заданное растровое изображение после его масштабирования до размера указанного прямоугольника. <br/> |



## <a name="remarks"></a>Remarks

Этот метод не возвращает код ошибки в случае сбоя. Чтобы определить, не завершилась ли операция рисования (например, **дравбитмап**), проверьте результат, возвращенный методами [**ID2D1RenderTarget:: EndDraw**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-enddraw) или [**ID2D1RenderTarget:: Flush**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-flush) .

## <a name="examples"></a>Примеры

Пример см. в разделе [Рисование растрового изображения](how-to-draw-a-bitmap.md). Пример загрузки точечного рисунка из ресурса или файла см. в разделе [Загрузка растрового](how-to-load-a-bitmap-from-a-resource.md) изображения из ресурса и [Загрузка растрового изображения из файла](how-to-load-a-direct2d-bitmap-from-a-file.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-------------------------------------------------------------------------------------|
| Библиотека<br/> | <dl> <dt>D2d1. lib</dt> </dl> |
| DLL<br/>     | <dl> <dt>D2d1.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ID2D1RenderTarget**](/windows/win32/api/d2d1/nn-d2d1-id2d1rendertarget)
</dt> <dt>

[Рисование точечного рисунка](how-to-draw-a-bitmap.md)
</dt> <dt>

[Как загрузить точечный рисунок из ресурса](how-to-load-a-bitmap-from-a-resource.md)
</dt> <dt>

[Как загрузить точечный рисунок из файла](how-to-load-a-direct2d-bitmap-from-a-file.md)
</dt> </dl>

 

