---
title: Инструкции по программированию для HLSL
description: Данные поступают в конвейер графики в виде потока примитивов и обрабатываются этапами шейдера.
ms.assetid: 4894e085-30e7-4cc5-8ae6-a84b601e4ce3
ms.topic: article
ms.date: 02/21/2019
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: cd242efaaf3cdb44f424a603f2fc522dda540ec8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127258448"
---
# <a name="programming-guide-for-hlsl"></a>Инструкции по программированию для HLSL

Данные поступают в конвейер графики в виде потока примитивов и обрабатываются этапами шейдера. Фактические этапы шейдера зависят от версии Direct3D, но, безусловно, включают в себя этапы вершин, точек и геометрических объектов. Другие этапы включают в себя поверхности и шейдеры доменов для тесселяции и шейдер вычислений. Эти этапы полностью программируемы с помощью языка штриховки высокого уровня ([HLSL](dx-graphics-hlsl-reference.md)).

Шейдеры HLSL можно компилировать на этапе разработки или во время выполнения, а также установить во время выполнения на соответствующий этап конвейера. Шейдеры Direct3D 9 можно разрабатывать с помощью [Shader Model 1](dx-graphics-hlsl-sm1.md), [Shader Model 2](dx-graphics-hlsl-sm2.md) и [Shader Model 3](dx-graphics-hlsl-sm3.md); Шейдер Direct3D 10 можно разрабатывать только на [Shader Model 4](dx-graphics-hlsl-sm4.md). Шейдер Direct3D 11 можно разрабатывать на [модели построителя текстуры 5](d3d11-graphics-reference-sm5.md). Direct3D 11,3 и Direct3D 12 можно разрабатывать на [модели шейдеров 5,1](shader-model-5-1.md), а Direct3D 12 также можно разрабатывать на [модели шейдеров 6](shader-model-6-0.md).

## <a name="in-this-section"></a>В этом разделе

| Раздел | Описание |
|-|-|
| [Использование связывания шейдера](using-shader-linking.md) | Мы покажем, как создавать предварительно скомпилированные функции HLSL, упаковывать их в библиотеки и связывать их с полными шейдерами во время выполнения. |
| [Создание шейдеров HLSL в Direct3D 9](dx-graphics-hlsl-writing-shaders-9.md) | |
| [Использование шейдеров в Direct3D 9](dx-graphics-hlsl-using-shaders-9.md) | |
| [Использование шейдеров в Direct3D 10](dx-graphics-hlsl-using-shaders-10.md) | |
| [Оптимизация шейдеров HLSL](dx-graphics-hlsl-optimize.md) | |
| [Отладка шейдеров в Visual Studio](dx-graphics-hlsl-debug-visual-studio.md) | новейшее средство для отладки шейдеров теперь поставляется как функция в Microsoft Visual Studio, называемая Visual Studio графическим отладчиком.  |
| [Компиляция шейдеров](dx-graphics-hlsl-part1.md) | Теперь рассмотрим различные способы компиляции кода шейдера и соглашений для расширений файлов для кода шейдера. |
| [Указание целевых объектов компилятора](specifying-compiler-targets.md) | Здесь перечислены целевые объекты для различных профилей, которые поддерживаются функциями **D3DCompile \*** и компилятором HLSL. |
| [Распаковка и \_ формат упаковки для редактирования образа In-Place](dx-graphics-hlsl-unpacking-packing-dxgi-format.md) | |
| [Использование HLSL минимальной точности](using-hlsl-minimum-precision.md) | начиная с Windows 8, графические драйверы могут реализовывать [скалярные типы данных](dx-graphics-hlsl-scalar.md) с минимальной точностью HLSL, используя любую точность, которая больше или равна заданной точности разрядов.  |
| [Модель шейдера HLSL 5](overviews-direct3d-11-hlsl.md) | |
| [Модель шейдера HLSL 5,1](hlsl-shader-model-5-1-features-for-direct3d-12.md) | В этом разделе описываются возможности модели шейдеров 5,1, применяемые на практике к D3D12 и D3D 11.3. Все оборудование DirectX 12 поддерживает модель шейдера 5,1. |
| [HLSL Shader Model 6.0](hlsl-shader-model-6-0-features-for-direct3d-12.md) | Описывает встроенные функции для операций Wave, добавленные в модель шейдера HLSL 6,0. |
| [Модель шейдера HLSL 6,4](hlsl-shader-model-6-4-features-for-direct3d-12.md) | Описывает встроенные функции машинного обучения, добавленные в модель шейдера HLSL 6,4. |

## <a name="related-topics"></a>Связанные темы

* [HLSL](dx-graphics-hlsl.md)
* [Справочник по HLSL](dx-graphics-hlsl-reference.md)
