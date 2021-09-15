---
title: Метод ID3DX11EffectTechnique Жетаннотатионбиндекс (D3dx11effect. h)
description: Получение заметки по индексу. | Метод ID3DX11EffectTechnique Жетаннотатионбиндекс (D3dx11effect. h)
ms.assetid: 703663b0-ee00-4686-a038-6c99ce61266b
keywords:
- Метод Жетаннотатионбиндекс Direct3D 11
- Метод Жетаннотатионбиндекс Direct3D 11, интерфейс ID3DX11EffectTechnique
- Интерфейс ID3DX11EffectTechnique Direct3D 11, метод Жетаннотатионбиндекс
topic_type:
- apiref
api_name:
- ID3DX11EffectTechnique.GetAnnotationByIndex
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e30712ba38f1360a992a8e409c249a746cca036
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127581227"
---
# <a name="id3dx11effecttechniquegetannotationbyindex-method"></a>Метод ID3DX11EffectTechnique:: Жетаннотатионбиндекс

Получение заметки по индексу.

## <a name="syntax"></a>Синтаксис


```C++
ID3DX11EffectVariable* GetAnnotationByIndex(
   UINT Index
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Index* 
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Отсчитываемый от нуля индекс указателя интерфейса.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **ID3DX11EffectVariable**](id3dx11effectvariable.md)\***

Указатель на [**ID3DX11EffectVariable**](id3dx11effectvariable.md).

## <a name="remarks"></a>Remarks

Используйте заметку, чтобы присоединить часть метаданных к приему.

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DX11EffectTechnique](id3dx11effecttechnique.md)
</dt> </dl>

 

