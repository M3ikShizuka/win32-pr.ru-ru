---
title: 'Функция Самплеград:: Самплеград (S, float, float, float, int, float, uint) для Texture3D'
description: Узнайте, как эта функция выбирает текстуру с помощью градиента, влияющей на способ вычисления расположения выборки, с необязательным значением для фиксации значения уровня детализации (Лод) в. Для Texture3D.
ms.assetid: 4B02A3B8-8179-497D-BF87-489BF0B9ECC2
keywords:
- Функция Самплеград HLSL
topic_type:
- apiref
api_name:
- SampleGrad
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 9bad18cb087bf18a779d371ee5daf78f03b707de1801d197d99b3ff590b343ee
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120023144"
---
# <a name="samplegradsamplegradsfloatfloatfloatintfloatuint-function-for-texture3d"></a>Функция Самплеград:: Самплеград (S, float, float, float, int, float, uint) для Texture3D

Выбор текстуры с помощью градиента, влияющей на способ вычисления расположения выборки, с дополнительным значением для фиксации значений уровня детализации (Лод). Возвращает состояние операции.

## <a name="syntax"></a>Синтаксис


``` syntax
DXGI_FORMAT SampleGrad(
  in  SamplerState S,
  in  float        Location,
  in  float        DDX,
  in  float        DDY,
  in  int          Offset,
  in  float        Clamp,
  out uint         Status
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*S* \[ в\]
</dt> <dd>

Тип: **самплерстате**

[Состояние образца](dx-graphics-hlsl-sampler.md). Это объект, объявленный в файле эффектов, который содержит назначения состояний.

</dd> <dt>

*Расположение* \[ окне\]
</dt> <dd>

Тип: **float**

Координаты текстуры. Тип аргумента зависит от типа объекта текстуры.



| Тип Texture-Object                    | Тип параметра |
|----------------------------------------|----------------|
| Texture1D                              | FLOAT          |
| Texture1DArray, Texture2D              | float2         |
| Texture2DArray, Texture3D, Текстурекубе | float3         |
| текстурекубеаррай                       | float4         |



 

</dd> <dt>

*DDX* \[ в\]
</dt> <dd>

Тип: **float**

Интенсивность изменения геометрии поверхности в направлении x. Тип аргумента зависит от типа объекта текстуры.



| Тип Texture-Object                      | Тип параметра |
|------------------------------------------|----------------|
| Texture1D, Texture1DArray                | FLOAT          |
| Texture2D, Texture2DArray                | float2         |
| Texture3D, Текстурекубе, Текстурекубеаррай | float3         |
| Texture2DMS, Texture2DMSArray            | Не поддерживается  |



 

</dd> <dt>

*ДДИ* \[ окне\]
</dt> <dd>

Тип: **float**

Интенсивность изменения геометрии поверхности в направлении y. Тип аргумента зависит от типа объекта текстуры.



| Тип Texture-Object                      | Тип параметра |
|------------------------------------------|----------------|
| Texture1D, Texture1DArray                | FLOAT          |
| Texture2D, Texture2DArray                | float2         |
| Texture3D, Текстурекубе, Текстурекубеаррай | float3         |
| Texture2DMS, Texture2DMSArray            | Не поддерживается  |



 

</dd> <dt>

*Смещение* \[ окне\]
</dt> <dd>

Тип: **int**

Необязательное Смещение координаты текстуры, которое может использоваться для любого типа объекта текстуры. смещение применяется к расположению перед выборкой. Используйте смещение только с целочисленным миплевел; в противном случае можно получить результаты, которые не могут быть правильно преобразованы в оборудование. Тип аргумента зависит от типа объекта текстуры. Дополнительные сведения см. в разделе [применение целочисленных смещений](dx-graphics-hlsl-to-sample.md).



| Тип Texture-Object           | Тип параметра |
|-------------------------------|----------------|
| Texture1D, Texture1DArray     | INT            |
| Texture2D, Texture2DArray     | int2           |
| Texture3D                     | int3           |
| Текстурекубе, Текстурекубеаррай | Не поддерживается  |



 

</dd> <dt>

*Срез* \[ окне\]
</dt> <dd>

Тип: **float**

Необязательное значение для примера среза Лод значений. Например, если передать значение среза 2.0 f, вы убедитесь, что ни один из отдельных примеров не имеет доступа к MIP уровню менее 2.0.

</dd> <dt>

*Состояние* \[ заполняет\]
</dt> <dd>

Тип: **uint**

Состояние операции. Вы не можете получить доступ к состоянию напрямую; Вместо этого передайте состояние в подставляемую функцию [**чеккакцессфуллимаппед**](checkaccessfullymapped.md) . **Чеккакцессфуллимаппед** возвращает **значение true** , если все значения из соответствующего **образца**, **сбора** или операции **загрузки** обращались к сопоставленным плиткам в [мозаичном ресурсе](/windows/desktop/direct3d11/direct3d-11-2-features). Если какие бы то ни было значения были взяты из несопоставленной плитки, **чеккакцессфуллимаппед** возвращает **значение false**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **\_ Формат DXGI**](/windows/desktop/api/dxgiformat/ne-dxgiformat-dxgi_format)**

Формат текстуры, который является одним из типизированных значений, перечисленных в [**\_ формате DXGI**](/windows/desktop/api/dxgiformat/ne-dxgiformat-dxgi_format).

## <a name="see-also"></a>См. также

<dl> <dt>

[Методы Самплеград](texture3d-samplegrad.md)
</dt> <dt>

[**Texture3D**](sm5-object-texture3d.md)
</dt> </dl>

 

 
