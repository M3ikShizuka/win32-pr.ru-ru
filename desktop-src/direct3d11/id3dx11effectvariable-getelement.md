---
title: Метод ID3DX11EffectVariable-Element (D3dx11effect. h)
description: Получение элемента массива.
ms.assetid: 3edf2084-570a-4423-8205-0b94a2a0cfde
keywords:
- Метод коэлемента Direct3D 11
- Метод коэлемента Direct3D 11, интерфейс ID3DX11EffectVariable
- Интерфейс ID3DX11EffectVariable Direct3D 11, метод WebMethod
topic_type:
- apiref
api_name:
- ID3DX11EffectVariable.GetElement
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9a5b887bb9e4c1d40f4d3eb0d36b9a7b4d2698b5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343003"
---
# <a name="id3dx11effectvariablegetelement-method"></a>Метод ID3DX11EffectVariable:: WebMethod

Получение элемента массива.

## <a name="syntax"></a>Синтаксис


```C++
ID3DX11EffectVariable* GetElement(
   UINT Index
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Index* 
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Отсчитываемый от нуля индекс; в противном случае — 0.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **ID3DX11EffectVariable**](id3dx11effectvariable.md)\***

Указатель на [**ID3DX11EffectVariable**](id3dx11effectvariable.md).

## <a name="remarks"></a>Remarks

Если переменная действия является массивом, используйте этот метод, чтобы вернуть один из элементов.

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DX11EffectVariable](id3dx11effectvariable.md)
</dt> </dl>

 

