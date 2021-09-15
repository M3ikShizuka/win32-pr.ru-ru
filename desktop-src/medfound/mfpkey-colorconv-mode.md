---
description: MFPKEY_COLORCONV_MODE свойство — указывает, является ли входной поток чередованием.
ms.assetid: d0d93151-5b0d-44a7-8497-f11b3e23a031
title: Свойство MFPKEY_COLORCONV_MODE (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a8c3f2d6256c4d7a9410264fb18703eea251e9c6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574870"
---
# <a name="mfpkey_colorconv_mode-property"></a>МФПКЭЙ \_ колорконв \_ mode, свойство

Указывает, является ли входной поток чередованием.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="default-value"></a>Значение по умолчанию

Вычислено DSP из исходного видео.

## <a name="applies-to"></a>Применяется к

-   [DSP цветового преобразователя](colorconverter.md)

## <a name="remarks"></a>Комментарии

Используйте одно из следующих значений.



| Значение | Описание |
|-------|-------------|
| 0     | прогрессивный |
| 2     | Interlaced  |



 

Если это свойство не задано, DSP использует входной тип носителя для определения, является ли видео чередованием. Это свойство можно задать, чтобы переопределить параметр типа мультимедиа.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 
