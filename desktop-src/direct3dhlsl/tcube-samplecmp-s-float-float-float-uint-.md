---
title: 'Функция Самплекмп:: Самплекмп (S, float, float, float, uint) для Текстурекубе'
description: 'Эта функция выбирает текстуру, используя значение сравнения для отклонения выборок, с необязательным значением для фиксации образцов значений уровня детализации (Лод) до. | Функция Самплекмп:: Самплекмп (S, float, float, float, uint) для Текстурекубе'
ms.assetid: 050E2856-1E93-4C69-8213-EEC082E82D40
keywords:
- Функция Самплекмп HLSL
topic_type:
- apiref
api_name:
- SampleCmp
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b73bf86b0c24feae87ea0bb4150d313fff604002
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066135"
---
# <a name="samplecmpsamplecmpsfloatfloatfloatuint-function-for-texturecube"></a>Функция Самплекмп:: Самплекмп (S, float, float, float, uint) для Текстурекубе

Выбор текстуры с использованием значения сравнения для отклонения выборок с необязательным значением для фиксации значений уровня детализации (Лод) в. Возвращает состояние операции.

## <a name="syntax"></a>Синтаксис


``` syntax
DXGI_FORMAT SampleCmp(
  in  SamplerState S,
  in  float        Location,
  in  float        CompareValue,
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

*Компаревалуе* \[ окне\]
</dt> <dd>

Тип: **float**

Значение с плавающей запятой, используемое в качестве значения сравнения.

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

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Методы Самплекмп](texturecube-samplecmp.md)
</dt> <dt>

[**текстурекубе**](texturecube.md)
</dt> </dl>

 

 
