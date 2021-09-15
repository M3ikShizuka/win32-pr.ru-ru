---
description: Указывает, каким способом в DSP записи голоса выполняется обработка массивов микрофона.
ms.assetid: 5e04fe50-d764-4497-9999-37279e156204
title: Свойство MFPKEY_WMAAECMA_FEATR_MICARR_MODE (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 25bf8ffcae465e8abfddedb3e6d6dded683bb2bf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462041"
---
# <a name="mfpkey_wmaaecma_featr_micarr_mode-property"></a>МФПКЭЙ \_ вмааекма \_ феатр \_ mode микарр, \_ свойство

Указывает, каким способом в DSP записи голоса выполняется обработка массивов микрофона.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="default-value"></a>Значение по умолчанию

\_ \_ однообразная микаррай

## <a name="applies-to"></a>Применяется к

-   [DSP для записи речи](voicecapturedmo.md)

## <a name="remarks"></a>Remarks

Значение этого свойства является членом перечисления [ \_ \_ режима массива MIC](/windows/desktop/api/wmcodecdsp/ne-wmcodecdsp-mic_array_mode) . Значение по умолчанию — МИКАРРАЙ \_ Single- \_ образная. Перед установкой этого свойства необходимо присвоить свойству [ \_ \_ \_ режима компонента мфпкэй вмааекма](mfpkey-wmaaecma-feature-modeproperty.md) значение Variant \_ true.

DSP использует это свойство только в том случае, если включена обработка массива микрофона.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> <dt>

[DSP для записи речи](voicecapturedmo.md)
</dt> </dl>

 

 
