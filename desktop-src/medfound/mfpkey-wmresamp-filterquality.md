---
description: Задает качество вывода.
ms.assetid: 7b45633b-7f1c-4951-a462-ad6240b9ca31
title: Свойство MFPKEY_WMRESAMP_FILTERQUALITY (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c4027d4bc3c0306240986cf632e171fa9a59ed18
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462034"
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

 

 
