---
title: WMT_VIDEOIMAGE_TRANSITION_BOW_TIE (Вмсдкидл. h)
description: Переход «линия бабочки» раскрывает новый образ в наборе треугольников на противоположных сторонах рамки.
ms.assetid: d98da767-eea7-460c-ae5f-6bef9d93ad9d
keywords:
- WMT_VIDEOIMAGE_TRANSITION_BOW_TIE формат Windows Media
topic_type:
- apiref
api_name:
- WMT_VIDEOIMAGE_TRANSITION_BOW_TIE
api_location:
- wmsdkidl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 45b61314709f6b0000281ac54e10f8aa702a9b24
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122471520"
---
# <a name="wmt_videoimage_transition_bow_tie"></a>ВМТ \_ видеоимаже \_ Переход на \_ бабочку \_

Переход «линия бабочки» раскрывает новый образ в наборе треугольников на противоположных сторонах рамки.

## <a name="parameters"></a>Параметры

В следующей таблице описаны параметры, используемые этим переходом, и перечислены члены структуры [**ВМТ \_ видеоимаже \_ SAMPLE2**](/previous-versions/windows/desktop/api/Wmsdkidl/ns-wmsdkidl-wmt_videoimage_sample2) , которой они назначены.




| Параметр | Член структуры | Описание | 
|-----------|------------------|-------------|
| Ширина | <strong>fEffectPara0</strong> | Ширина каждой треугольной стороны для привязки бабочки. | 
| Высота | <strong>fEffectPara1</strong> | Высота каждой треугольной стороны привязку к бабочке. | 
| Направление | <strong>fEffectPara2</strong> | Задайте одно из следующих значений:<ul><li>0 — задает результат горизонтальной бабочки, в котором треугольники вводятся справа и слева от рамки.</li><li>1 — задает действие по вертикали, при котором треугольники вводятся сверху и снизу рамки.</li></ul> | 
| Композиция | <strong>fEffectPara3</strong> | Задайте одно из следующих значений:<ul><li>0 — задает нормальную композицию, в которой предыдущее изображение является фоном, а текущее изображение — передним планом.</li><li>1 — задает обратную композицию, в которой текущий рисунок является фоновым изображением, а предыдущее изображение — передний план.</li></ul> | 




 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Вмсдкидл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Переходы по изображениям видео**](video-image-transitions.md)
</dt> </dl>

 

 





