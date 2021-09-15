---
title: Тип вектора (HLSL)
description: Вектор содержит от одного до четырех скалярных компонентов; Каждый компонент вектора должен иметь один и тот же тип.
ms.assetid: 16e66f3c-c513-4d03-8adf-463dc8d83e12
keywords:
- Тип вектора HLSL
topic_type:
- apiref
api_name:
- Vector Type
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 76d07da5d22dfb44215f70a7620d6519b5c8a802
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573751"
---
# <a name="vector-type"></a>Тип вектора

Вектор содержит от одного до четырех скалярных компонентов; Каждый компонент вектора должен иметь один и тот же тип.



|                     |
|---------------------|
| **Имя Типенумбер** |



 


```
TypeComponents Name
```



## <a name="components"></a>Компоненты



| Элемент                                                                                                                             | Описание                                                                                                                                                                                                           |
|----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="TypeComponents"></span><span id="typecomponents"></span><span id="TYPECOMPONENTS"></span>**типекомпонентс**<br/> | Одно имя, содержащее две части. Первая часть является одним из [скалярных](dx-graphics-hlsl-data-types.md) типов. Вторая часть — это число компонентов, которое должно находиться в диапазоне от 1 до 4 включительно.<br/> |
| <span id="Name"></span><span id="name"></span><span id="NAME"></span>**Безымян**<br/>                                         | Строка ASCII, однозначно определяющая имя переменной.<br/>                                                                                                                                                |



 

## <a name="examples"></a>Примеры

Ниже приведены некоторые примеры:


```
bool    bVector;   // scalar containing 1 Boolean
int1    iVector = 1;
float3  fVector = { 0.2f, 0.3f, 0.4f };
```



Вектор можно объявить с помощью этого синтаксиса:


```
vector <Type, Number> VariableName
```



Ниже приведены некоторые примеры:


```
vector <int,    1> iVector = 1;
vector <double, 4> dVector = { 0.2, 0.3, 0.4, 0.5 };
```

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Типы данных (DirectX HLSL)](dx-graphics-hlsl-data-types.md)
</dt> </dl>

 

 





