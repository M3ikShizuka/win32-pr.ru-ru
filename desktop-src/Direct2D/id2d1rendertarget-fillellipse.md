---
title: Методы Филлеллипсе ID2D1RenderTarget (D2d1. h)
description: Закрашивает внутреннюю часть указанного эллипса.
ms.assetid: 149fb303-d2e8-416c-b28f-8bc5f1482ba6
keywords:
- Методы Филлеллипсе Direct2D
topic_type:
- apiref
api_location:
- D2d1.dll
api_type:
- DllExport
ms.date: 07/02/2019
ms.topic: reference
ms.openlocfilehash: 7ee6624e5f557bb82924b4fa0f77d88a9cec35775a72009608120e8b8f2bd063
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119874174"
---
# <a name="id2d1rendertargetfillellipse-methods"></a>Методы ID2D1RenderTarget:: Филлеллипсе

Закрашивает внутреннюю часть указанного эллипса.

### <a name="overload-list"></a>Список перегрузок



| Метод                                                                                                             | Описание                                               |
|:-------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------|
| [**Филлеллипсе (D2D1 \_ ellipse&, ID2D1Brush \* )**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-fillellipse(constd2d1_ellipse__id2d1brush))  | Закрашивает внутреннюю часть указанного эллипса. <br/> |
| [**Филлеллипсе (D2D1 \_ Ellipse \* , ID2D1Brush \* )**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-fillellipse(constd2d1_ellipse__id2d1brush)) | Закрашивает внутреннюю часть указанного эллипса. <br/> |



## <a name="remarks"></a>Remarks

Этот метод не возвращает код ошибки в случае сбоя. Чтобы определить, не завершилась ли операция рисования (например, **филлеллипсе**), проверьте результат, возвращенный методами [**ID2D1RenderTarget:: EndDraw**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-enddraw) или [**ID2D1RenderTarget:: Flush**](/windows/win32/api/d2d1/nf-d2d1-id2d1rendertarget-flush) .

## <a name="examples"></a>Примеры

Пример см. в разделе [Рисование и заполнение базовой фигуры](how-to-draw-an-ellipse.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D2d1. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D2d1. lib</dt> </dl> |
| DLL<br/>     | <dl> <dt>D2d1.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ID2D1RenderTarget**](/windows/win32/api/d2d1/nn-d2d1-id2d1rendertarget)
</dt> <dt>

[Рисование и заполнение базовой фигуры](how-to-draw-an-ellipse.md)
</dt> </dl>

�

�
