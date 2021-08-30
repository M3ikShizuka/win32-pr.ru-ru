---
title: Метод ID3DX11EffectVariable Ассамплер (D3dx11effect. h)
description: Получить переменную образца.
ms.assetid: dff699f7-758a-442b-93eb-23a09468251f
keywords:
- Метод Ассамплер Direct3D 11
- Метод Ассамплер Direct3D 11, интерфейс ID3DX11EffectVariable
- Интерфейс ID3DX11EffectVariable Direct3D 11, метод Ассамплер
topic_type:
- apiref
api_name:
- ID3DX11EffectVariable.AsSampler
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7a6c71e8e2cdc89860c8edf82a0c008c03f4a154ab23cee882ed1e9eaaad2939
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119894604"
---
# <a name="id3dx11effectvariableassampler-method"></a>Метод ID3DX11EffectVariable:: Ассамплер

Получить переменную образца.

## <a name="syntax"></a>Синтаксис


```C++
ID3DX11EffectSamplerVariable* AsSampler();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **ID3DX11EffectSamplerVariable**](id3dx11effectsamplervariable.md)\***

Указатель на переменную образца. См. [**ID3DX11EffectSamplerVariable**](id3dx11effectsamplervariable.md).

## <a name="remarks"></a>Remarks

Ассамплер Возвращает версию переменной Effect, которая была специализированной для переменной образца. Как и в приведении, эта специализация вернет недопустимый объект, если переменная действия не содержит данные выборки.

Приложения могут проверить возвращаемый объект на допустимость, вызвав [**IsValid**](id3dx11effectvariable-isvalid.md).

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DX11EffectVariable](id3dx11effectvariable.md)
</dt> </dl>

 

 





