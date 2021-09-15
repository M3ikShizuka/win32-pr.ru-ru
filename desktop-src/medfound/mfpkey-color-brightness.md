---
description: Корректирует яркость.
ms.assetid: 1b3f56eb-3f22-4120-ba6c-331eccd5d303
title: Свойство MFPKEY_COLOR_BRIGHTNESS (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 685ab934a91f1843183fcfa88bb94c83e602db27
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580307"
---
# <a name="mfpkey_color_brightness-property"></a>МФПКЭЙ \_ , \_ свойство яркости цвета

Корректирует яркость.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="default-value"></a>Значение по умолчанию

0

## <a name="applies-to"></a>Применяется к

-   [Преобразование элемента управления цветом DSP](colorcontroltransform.md)

## <a name="remarks"></a>Remarks

Корректировка яркости выполняется путем добавления значения в канал яркости.

Это свойство имеет диапазон от-127 до 127. Ноль означает отсутствие изменений в яркости.

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

 

 
