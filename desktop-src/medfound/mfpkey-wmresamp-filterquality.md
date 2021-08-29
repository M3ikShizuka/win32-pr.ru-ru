---
description: Задает качество вывода.
ms.assetid: 7b45633b-7f1c-4951-a462-ad6240b9ca31
title: Свойство MFPKEY_WMRESAMP_FILTERQUALITY (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9bf00b757bd07add37f6a5b82459f37df40f9fb36ea6ef813e011adcadde196e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119603374"
---
# <a name="mfpkey_wmresamp_filterquality-property"></a>МФПКЭЙ \_ вмресамп \_ Филтеркуалити, свойство

Задает качество вывода.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="applies-to"></a>Применяется к

-   [DSP по интерполяции аудио](audioresampler.md)

## <a name="remarks"></a>Remarks

Допустимый диапазон этого свойства — от 1 до 60 включительно. Чем больше значение, тем выше качество вывода, но тем больше задержка. Значение 1 по сути совпадает с линейной интерполяцией.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 
