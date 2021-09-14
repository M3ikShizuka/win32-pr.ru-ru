---
title: Эффект смешивания
description: Используйте эффекты смешения для объединения двух изображений. Этот результат имеет 26 режимов смешения.
ms.assetid: 39D8BAA3-8FF3-4F10-99A0-B26FCA3018AE
keywords:
- эффекты смешения
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 853043123c6eea9a87656a7450b1295236ed5d6a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127164244"
---
# <a name="blend-effect"></a>Эффект смешивания

Используйте эффекты смешения для объединения двух изображений. Этот результат имеет 26 режимов смешения.

Идентификатором CLSID для этого действия является CLSID \_ D2D1Blend.

-   [Примеры смешения](#blending-examples)
-   [Свойства эффектов](#effect-properties)
-   [Режимы смешения](#blend-modes)
-   [HSL. преобразование цветового пространства](#hsl-color-space-conversions)
    -   [Преобразование RGB в HSL](#converting-from-rgb-to-hsl)
    -   [Преобразование из HSL в RGB](#converting-from-hsl-to-rgb)
-   [Битовая карта вывода](#output-bitmap)
-   [Образец кода](#sample-code)
-   [Requirements](#requirements)
-   [Связанные темы](#related-topics)

## <a name="blending-examples"></a>Примеры смешения

Ниже приведен пример изображения для каждого режима наложения в результате смешения. Полный список режимов наложения и соответствующих свойств режима см. в следующем разделе.

![снимок экрана с примерами эффектов для всех доступных режимов наложения.](images/blend-modes.png)

Ниже приведен еще один пример использования режима исключения.



| До образа 1                                                             |
|----------------------------------------------------------------------------|
| ![Первое исходное изображение перед результатом.](images/default-before.jpg)    |
| До изображения 2                                                             |
| ![Второе изображение перед результатом.](images/4-arthimetic-composite2.jpg) |
| После                                                                      |
| ![изображение после преобразования.](images/5-blend.png)                      |



 


```C++
ComPtr<ID2D1Effect> blendEffect;
m_d2dContext->CreateEffect(CLSID_D2D1Blend, &blendEffect);

blendEffect->SetInput(0, bitmap);
blendEffect->SetInput(1, bitmapTwo);
blendEffect->SetValue(D2D1_BLEND_PROP_MODE, D2D1_BLEND_MODE_EXCLUSION);

m_d2dContext->BeginDraw();
m_d2dContext->DrawImage(blendEffect.Get());
m_d2dContext->EndDraw();
```



## <a name="effect-properties"></a>Свойства эффектов



| Отображаемое имя и перечисление индекса                 | Описание                                                                                                                                                                               |
|----------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Режим<br/> \_Режим D2D1 \_ Blend \_<br/> | Режим смешения, используемый для этого результата. Дополнительные сведения см. в разделе [режимы смешения](#blend-modes) . Тип — D2D1 \_ Blend \_ .<br/> Значение по умолчанию — \_ D2D1 \_ Blend \_ .<br/> |



 

## <a name="blend-modes"></a>Режимы смешения

В таблице здесь показаны все режимы наложения этого результата. Вспомогательные функции, необходимые для расчета выходных данных этого результата, приведены в следующем разделе.

Цвет: O <sub>пргб</sub>  =  *f*(f <sub>RGB</sub>, B <sub>RGB</sub>) \* f <sub>a</sub> \* B <sub>а</sub> + f <sub>RGB</sub> \* f <sub>a</sub> \* (1-B <sub>а</sub>) + B <sub>RGB</sub> \* B <sub>A</sub> \* (1 – f <sub>a</sub>)

Альфа: O<sub>a</sub> = F<sub>A</sub> \* (1-B<sub>а</sub>) + B<sub>a</sub>

Где:

-   O<sub>пргб</sub> — это предварительно умноженный выходной цвет
-   O<sub>A</sub> является выходным альфа-каналом
-   B<sub>RGB</sub> — это непредварительно умноженный цвет назначения
-   Б<sub>— альфа-канал</sub> назначения
-   F<sub>RGB</sub> — это непредварительно умноженный исходный цвет
-   F<sub>A</sub> — это альфа-версия источника
-   *f*(<sub>RGB</sub>, D <sub>RGB</sub>) — это функция Blend, которая изменяется в зависимости от режима смешения

Для некоторых режимов наложения требуется преобразование из цветового пространства оттенки, насыщенности, яркости (HSL) в RGB и обратно.




| Перечисление | Дробь | 
|-------------|----------|
| D2D1_BLEND_MODE_DARKEN | Базовая формула Blend только для Alpha. <img src="images/blend-mode-darken-1.png" alt="mathematical formula for a darken effect." /> | 
| D2D1_BLEND_MODE_MULTIPLY | Базовая формула Blend только для Alpha. <img src="images/blend-mode-multiply-1.png" alt="Mathematical formula for a mutiply effect." /> | 
| D2D1_BLEND_MODE_COLOR_BURN | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-colorburn-1.png" alt="Mathematical formula for a coor burn effect." /> | 
| D2D1_BLEND_MODE_LINEAR_BURN | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-linearburn-1.png" alt="Mathematical formula for a linear burn effect." /> | 
| D2D1_BLEND_MODE_DARKER_COLOR | Базовая формула Blend только для Alpha. <img src="images/blend-mode-darkencolor-1.png" alt="Mathematical formla for a darken color effect." /> | 
| D2D1_BLEND_MODE_LIGHTEN | Базовая формула Blend только для Alpha. <img src="images/blend-mode-lighten-1.png" alt="Mathematical formula for a lighten effect." /> | 
| D2D1_BLEND_MODE_SCREEN | Базовая формула Blend только для Alpha. <img src="images/blend-mode-screen-1.png" alt="Mathematical formula for a screen effect." /> | 
| D2D1_BLEND_MODE_COLOR_DODGE | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-colordodge-1.png" alt="Mathematical formula for a color dodge effect." /> | 
| D2D1_BLEND_MODE_LINEAR_DODGE | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-lineardodge-1.png" alt="Mathematical formula for a linear dodge effect." /> | 
| D2D1_BLEND_MODE_LIGHTER_COLOR | Базовая формула Blend только для Alpha. <img src="images/blend-mode-lightercolor-1.png" alt="Mathematical formula for a lighter color effect." /> | 
| D2D1_BLEND_MODE_OVERLAY | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-overlay-1.png" alt="Mathematical formula for an overlay effect." /> | 
| D2D1_BLEND_MODE_SOFT_LIGHT | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-softlight-1.png" alt="Mathematical formula for a soft light effect." /> | 
| D2D1_BLEND_MODE_HARD_LIGHT | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-hardlight-1.png" alt="Mathematical formula for a hard light effect." /> | 
| D2D1_BLEND_MODE_VIVID_LIGHT | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-vividlight-1.png" alt="Mathematical formula for a vivid light effect." /> | 
| D2D1_BLEND_MODE_LINEAR_LIGHT | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-linearlight-1.png" alt="Mathematical formula for a linear light effect." /> | 
| D2D1_BLEND_MODE_PIN_LIGHT | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-pinlight-1.png" alt="Mathematical formula for a pin light effect." /> | 
| D2D1_BLEND_MODE_HARD_MIX | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = <img src="images/blend-mode-hardmix-1.png" alt="Mathematical formula for a hard mix effect." /> | 
| D2D1_BLEND_MODE_DIFFERENCE | Основные формулы смешения с <em>f</em>(f<sub>RGB</sub>, B<sub>RGB</sub>) = ABS (f<sub>RGB</sub> -b<sub>RGB</sub>) | 
| D2D1_BLEND_MODE_EXCLUSION | Основные формулы смешения <em>с f</em>(<sub>f RGB</sub>, b<sub>RGB</sub>) = f<sub>RGB</sub> + b<sub>RGB</sub>   2 * f<sub>RGB</sub> * B<sub>RGB</sub> | 
| D2D1_BLEND_MODE_HUE | Базовая формула Blend только для Alpha. <img src="images/blend-mode-hue-1.png" alt="Mathematical formula for a hue blend effect." /> | 
| D2D1_BLEND_MODE_SATURATION | Базовая формула Blend только для Alpha. <img src="images/blend-mode-saturation-1.png" alt="Mathematical formula for a sturation blend effect." /> | 
| D2D1_BLEND_MODE_COLOR | Базовая формула Blend только для Alpha. <img src="images/blend-mode-color-1.png" alt="Mathematical formula for a color blend effect." /> | 
| D2D1_BLEND_MODE_LUMINOSITY | Базовая формула Blend только для Alpha. <img src="images/blend-mode-luminosity-1.png" alt="Mathematical formula for a luminosity blend effect." /> | 
| D2D1_BLEND_MODE_DISSOLVE | Исходные данные:<ul><li>ТОЧЕЧная координата сцены для текущего пикселя</li><li>Детерминированный генератор случайных чисел Rand (XY), основанный на координатах начальной координаты, с несмещенным распределением значений из [0, 1]</li></ul><br /><img src="images/blend-mode-dissolve-1.png" alt="Mathematical formula for a dissolve blend effect." /><br /> | 
| D2D1_BLEND_MODE_SUBTRACT | Базовая формула Blend только для Alpha. <img src="images/blend-mode-subtract-1.png" alt="Mathematical formula for a subtract blend effect." /> | 
| D2D1_BLEND_MODE_DIVISION | Базовая формула Blend только для Alpha. <img src="images/blend-mode-division-1.png" alt="Mathematical formula for a division blend effect." /> | 




 

> [!Note]  
> Для всех режимов наложения выходное значение предварительно умножается и замещается в диапазон \[ 0, 1 \] .

 

## <a name="hsl-color-space-conversions"></a>HSL. преобразование цветового пространства

Компонент "яркость" вычисляются с использованием веса RGB здесь:

-   *k*<sub>R</sub> = 0,30
-   *k*<sub>G</sub> = 0,59
-   *k*<sub>б</sub> = 0,11

### <a name="converting-from-rgb-to-hsl"></a>Преобразование RGB в HSL

![Математическая формула, описывающая преобразование цвета RGB в значение HSL Color.](images/blend-rgb-to-hsl-1.png)

Это помещает *S* и *L* в диапазоне \[ 0,0, 1,0 \] и *H* в диапазоне \[ -1,0, 5,0 \] .

### <a name="converting-from-hsl-to-rgb"></a>Преобразование из HSL в RGB

Для преобразования другого способа используется обратная часть предыдущих вычислений.

Если *S* = 0, то *R*  =  *G*  =  *B*  =  *L*

В противном случае есть шесть вариантов, зависимых от оттенок:

Если значение *H* больше 0, значения находятся в красно-пурпурном секторе, где *R*  >  *B*  >  *G*.

![математический екуаитон шаг 1 из шести преобразований цвета HSL в RGB.](images/blend-hsl-to-rgb-1rm.png)

Если значение *H* больше или равно 0 и меньше 1, значения находятся в красно-желтом секторе, где *R*  >  *G*  >  *B*.

![математический екуаитон шаг 2 из шести преобразований цвета HSL в RGB.](images/blend-hsl-to-rgb-1ry.png)

Если *H* больше или равно 1 и меньше 2, значения находятся в желтом/зеленом секторе, где *G*  >  *R*  >  *B*.

![математический екуаитон шаг 3 из шести преобразований цвета HSL в RGB.](images/blend-hsl-to-rgb-1yg.png)

Если *H* больше или равно 2 и меньше 3, значения находятся в зеленом/голубом секторе, где *G*  >  *B*  >  *R*.

![математически екуаитон шаг 4 из шести преобразований цвета HSL в RGB.](images/blend-hsl-to-rgb-1gc.png)

Если значение *H* больше или равно 3 и меньше 4, значения находятся в голубом/синем секторе, где *B*  >  *G*  >  *R*.

![математически екуаитон шаг 5 из шести преобразований цвета HSL в RGB.](images/blend-hsl-to-rgb-1cb.png)

Если *H* больше или равно 4, значения находятся в синем/пурпурном секторе, где *B*  >  *R*  >  *G*.

![математически екуаитон шаг шесть из шести преобразований цвета HSL в RGB.](images/blend-hsl-to-rgb-1bm.png)

Поскольку режимы наложения выполняют произвольные сочетания компонентов HSL из двух разных цветов, то обычно преобразованное значение RGB становится недопустимым, то есть один или несколько компонентов канала могут находиться за пределами допустимого диапазона \[ 0,0, 1,0 \] . Эти цвета возвращаются в цветовой охват путем минимального уменьшения насыщенности, сохраняя как оттенок, так и яркость:

![Математическая формула, описывающая исправления, необходимые для использования экземпляров цветового охвата.](images/blend-gamut-correction.png)

## <a name="output-bitmap"></a>Битовая карта вывода

Выходным точечным рисунком для этого результата всегда является размер объединения двух входных изображений.

## <a name="sample-code"></a>Образец кода

Чтобы получить пример этого результата, скачайте [образец Direct2D составных эффектов](https://github.com/microsoftarchive/msdn-code-gallery-microsoft/tree/master/Official%20Windows%20Platform%20Sample/Direct2D%20composite%20effect%20modes%20sample).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента | Windows 8 и обновление платформы для Windows 7 \[ классических приложений \| Windows приложения магазина\] |
| Минимальная версия сервера | Windows 8 и обновление платформы для Windows 7 \[ классических приложений \| Windows приложения магазина\] |
| Заголовок                   | d2d1effects. h                                                                      |
| Библиотека                  | D2D1. lib, дксгуид. lib                                                               |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**ID2D1Effect**](/windows/win32/api/d2d1_1/nn-d2d1_1-id2d1effect)
</dt> </dl>

 

