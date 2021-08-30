---
title: dcl_input_sv (SM4-ASM)
description: дкл \_ входной \_ ОКП (SM4-ASM)
ms.assetid: 59270148-e2eb-4525-a888-ad7e843d62a5
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: b703677bb4e99f70443c89a8f907fa7abfaaff11
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122481270"
---
# <a name="dcl_input_sv-sm4---asm"></a>дкл \_ входной \_ ОКП (SM4-ASM)

Объявляет входной регистр шейдера, который ждет, что [системное значение](dx-graphics-hlsl-semantics.md) должно быть предоставлено из предыдущего этапа.



| дкл \_ входной \_ ОКП v *N \[ . Mask \]*, *системвалуенаме \[ , интерполатионмоде \]* |
|------------------------------------------------------------------------|



 




| Элемент | Описание | 
|------|-------------|
| <span id="vN_.mask_"></span><span id="vn_.mask_"></span><span id="VN_.MASK_"></span>v<em>N [. Маска]</em><br /> | окне Регистр данных вершин. <br /><ul><li><em>N</em> — это целое число, определяющее номер регистра.</li><li><em>[. Mask]</em> — это необязательная маска компонента (. ксизв), указывающая, какие компоненты регистров следует использовать.</li></ul> | 
| <span id="systemValueName"></span><span id="systemvaluename"></span><span id="SYSTEMVALUENAME"></span><em>системвалуенаме</em><br /> | окне Имя системного значения, которое является строкой (см. раздел <a href="dx-graphics-hlsl-semantics.md">семантика системного значения</a>) без префикса "SV_".<br /> | 
| <span id="interpolationMode"></span><span id="interpolationmode"></span><span id="INTERPOLATIONMODE"></span><em>интерполатионмоде</em><br /> | [в] Необязательно. Режим интерполяции, который влияет на способ вычисления значений во время растрирования; режим используется только в шейдере пикселей. Может иметь одно из следующих значений. <br /><ul><li>Константа — не выполнять интерполяцию между значениями регистров.</li><li>линейная — линейная интерполяция между значениями регистра.</li><li>Линеарцентроид — то же, что и линейный, но центроид при множественной выборке.</li><li>Линеарноперспективе — то же, что и линейная, но без исправления перспективы.</li><li>Линеарноперспективецентроид — то же, что и линейная, но без изменений перспективы и центроид при множественной выборки.</li></ul> | 




 

Маска компонента для объявления системного значения может быть любым подмножеством \[ ксизв \] ; объявления не могут перекрываться (каждое объявление должно следовать за последовательностью ксизв). При объявлении скалярных системных значений (например, расстояния обрезки и расстояния для отбора) можно объявить несколько системных значений в одном регистре. В этом случае убедитесь, что другие модификаторы, такие как режимы интерполяции, совпадают.

Эта инструкция применяется к следующим этапам шейдера:



| Вершинный построитель текстуры | Шейдер геометрии | Построитель текстуры |
|---------------|-----------------|--------------|
| x             | x               | x            |



 

Эта инструкция включена для облегчения отладки шейдера в сборке; нельзя создать шейдер на языке ассемблера с использованием модели шейдеров 4.

## <a name="example"></a>Пример

Ниже приводится несколько примеров.


```
// valid
dcl_input v0.y, linear
dcl_input_sv v0.w, clipDistance
dcl_input_sv v0.z, cullDistance
```




```
// invalid declarations
dcl_input v0.y, linear
dcl_input_sv v0.x, clipDistance  // the y component was previously declared, this declaration must use 
                                 // either the z or w component

dcl_input v0.y, linearNoPerspective                  // the interpolation mode is linear-no-perspective
dcl_input_sv v0.z, renderTargetArrayIndex, constant  // the interpolation modes is constant
                                                     // the interpolation modes must match
```



## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                              | Поддерживается |
|-----------------------------------------------------------|-----------|
| [Модель шейдера 5](d3d11-graphics-reference-sm5.md)        | Да       |
| [Модель шейдера 4,1](dx-graphics-hlsl-sm4.md)              | Да       |
| [Модель шейдера 4](dx-graphics-hlsl-sm4.md)                | Да       |
| [Модель шейдера 3 (DirectX HLSL)](dx-graphics-hlsl-sm3.md) | Нет        |
| [Модель шейдера 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) | Нет        |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md) | Нет        |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сборка Shader Model 4 (DirectX HLSL)](dx-graphics-hlsl-sm4-asm.md)
</dt> </dl>

 

 





