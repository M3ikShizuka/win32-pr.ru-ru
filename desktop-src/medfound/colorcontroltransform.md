---
description: Регулирует цветовые характеристики потока видео.
ms.assetid: 738c1f0c-8417-4b12-a7f1-9bbf3c7e9dd3
title: Преобразование элемента управления цветом DSP (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0b94c8314bfd2be85a3bbc392bfa0e83767ff0b0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257960"
---
# <a name="color-control-transform-dsp"></a>Преобразование элемента управления цветом DSP

Регулирует цветовые характеристики потока видео.

## <a name="clsid"></a>CLSID

\_ККОЛОРКОНТРОЛДМО CLSID

## <a name="interfaces"></a>Интерфейсы

-   **имедиаобжект**
-   **имфтрансформ**
-   **ипропертисторе**

## <a name="formats"></a>Форматы

-   RGB 24
-   RGB 32
-   RGB 555
-   RGB 565
-   айув
-   UYVY
-   YUY2
-   YV12

## <a name="properties"></a>Свойства

-   [\_цветовая \_ яркость мфпкэй](mfpkey-color-brightness.md)
-   [\_ \_ контрастность цвета мфпкэй](mfpkey-color-contrast.md)
-   [\_цветовой \_ тон мфпкэй](mfpkey-color-hue.md)
-   [МФПКЭЙ \_ \_ насыщенность цвета](mfpkey-color-saturation.md)

## <a name="remarks"></a>Комментарии

Этот DSP изменяет содержимое потока видео. Для воспроизведения можно повысить эффективность аналогичных эффектов с помощью интерфейса **имфвидеопроцессор** , который управляет обработкой видео в графической карте.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Mfvdsp.dll</dt> </dl>   |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Обработчики цифровых сигналов](windowsmediadigitalsignalprocessors.md)
</dt> </dl>

 

 




