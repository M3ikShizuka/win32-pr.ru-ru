---
description: '\_ \_ Тип перечисления «исправленные \_ значения состояния WPD» \_ описывает состояние цветовой коррекции изображения или видеофайла.'
ms.assetid: af129a1b-7760-4339-adf7-3f3c17cebde2
title: Перечисление WPD_COLOR_CORRECTED_STATUS_VALUES (Портабледевице. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WPD_COLOR_CORRECTED_STATUS_VALUES
api_type:
- HeaderDef
api_location:
- PortableDevice.h
ms.openlocfilehash: 94caa345c0c7bee6c500109d6ebc6cbedd0aefae5254a254dbc5af907e0be737
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120089594"
---
# <a name="wpd_color_corrected_status_values-enumeration"></a>\_ \_ \_ Перечисление значений состояния ИСПРАВЛЕНного цвета WPD \_

Тип перечисления « **\_ \_ исправленные \_ \_ значения состояния WPD** » описывает состояние цветовой коррекции изображения или видеофайла.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum WPD_COLOR_CORRECTED_STATUS_VALUES { 
  WPD_COLOR_CORRECTED_STATUS_NOT_CORRECTED            = 0,
  WPD_COLOR_CORRECTED_STATUS_CORRECTED                = 1,
  WPD_COLOR_CORRECTED_STATUS_SHOULD_NOT_BE_CORRECTED  = 2
} ;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="WPD_COLOR_CORRECTED_STATUS_NOT_CORRECTED"></span><span id="wpd_color_corrected_status_not_corrected"></span>**\_ \_ Исправлено цветовое \_ состояние WPD \_ не \_ исправлено**
</dt> <dd>

Изображение не исправлено цветом.

</dd> <dt>

<span id="WPD_COLOR_CORRECTED_STATUS_CORRECTED"></span><span id="wpd_color_corrected_status_corrected"></span>**Исправлено \_ \_ состояние исправленного цвета WPD \_ \_**
</dt> <dd>

Изображение исправлено цветом.

</dd> <dt>

<span id="WPD_COLOR_CORRECTED_STATUS_SHOULD_NOT_BE_CORRECTED"></span><span id="wpd_color_corrected_status_should_not_be_corrected"></span>**\_ \_ Исправлено цветовое \_ состояние WPD \_ \_ не должно \_ быть \_ исправлено**
</dt> <dd>

Образ не был и не должен быть исправлен цветом.

</dd> </dl>

## <a name="remarks"></a>Remarks

Указывает состояние исправленного цвета изображения. Это перечисление используется свойством " [ \_ \_ \_ исправленное \_ состояние цветового изображения WPD](image-properties.md) ".

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Портабледевице. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Структуры и типы перечислений**](structures-and-enumeration-types.md)
</dt> </dl>

 

 




