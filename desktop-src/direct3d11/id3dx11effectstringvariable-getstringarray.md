---
title: Метод ID3DX11EffectStringVariable Жетстрингаррай (D3dx11effect. h)
description: Получение массива строк.
ms.assetid: 2cc45b2f-1851-49d2-8844-3e249c48f327
keywords:
- Метод Жетстрингаррай Direct3D 11
- Метод Жетстрингаррай Direct3D 11, интерфейс ID3DX11EffectStringVariable
- Интерфейс ID3DX11EffectStringVariable Direct3D 11, метод Жетстрингаррай
topic_type:
- apiref
api_name:
- ID3DX11EffectStringVariable.GetStringArray
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e88772edef9b975b34287b448b477e5ad2ada5cbf3f5f006dd76b8b9d158c3a
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119894904"
---
# <a name="id3dx11effectstringvariablegetstringarray-method"></a>Метод ID3DX11EffectStringVariable:: Жетстрингаррай

Получение массива строк.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetStringArray(
   LPCSTR *ppStrings,
   UINT   Offset,
   UINT   Count
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппстрингс* 
</dt> <dd>

Тип: **[ **LPCSTR**](/windows/desktop/WinProg/windows-data-types)\***

Указатель на первую строку в массиве.

</dd> <dt>

*Offset* 
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Смещение (в количестве строк) между началом массива и первой строкой, которую необходимо получить.

</dd> <dt>

*Количество* 
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Количество строк в возвращаемом массиве.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращает один из следующих [кодов возврата Direct3D 11](d3d11-graphics-reference-returnvalues.md).

## <a name="remarks"></a>Remarks

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DX11EffectStringVariable](id3dx11effectstringvariable.md)
</dt> </dl>

 

