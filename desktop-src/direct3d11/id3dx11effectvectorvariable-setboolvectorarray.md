---
title: Метод ID3DX11EffectVectorVariable Сетбулвектораррай (D3dx11effect. h)
description: Установите массив векторов из четырех компонентов, содержащих логические данные.
ms.assetid: 063735de-093c-4891-9a5c-fe1622da283b
keywords:
- Метод Сетбулвектораррай Direct3D 11
- Метод Сетбулвектораррай Direct3D 11, интерфейс ID3DX11EffectVectorVariable
- Интерфейс ID3DX11EffectVectorVariable Direct3D 11, метод Сетбулвектораррай
topic_type:
- apiref
api_name:
- ID3DX11EffectVectorVariable.SetBoolVectorArray
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0ce1f34783390c4bcef55df81ba6c9a2215486cb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056023"
---
# <a name="id3dx11effectvectorvariablesetboolvectorarray-method"></a>Метод ID3DX11EffectVectorVariable:: Сетбулвектораррай

Установите массив векторов из четырех компонентов, содержащих логические данные.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetBoolVectorArray(
   BOOL *pData,
   UINT Offset,
   UINT Count
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pData* 
</dt> <dd>

Тип: **[ **bool** .](/windows/desktop/WinProg/windows-data-types)\***

Указатель на начало данных, которые необходимо задать.

</dd> <dt>

*Offset* 
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Необходимо задать значение 0; это зарезервировано для будущего использования.

</dd> <dt>

*Количество* 
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Число заданных элементов массива.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращает один из следующих [кодов возврата Direct3D 11](d3d11-graphics-reference-returnvalues.md).

## <a name="remarks"></a>Комментарии

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[ID3DX11EffectVectorVariable](id3dx11effectvectorvariable.md)
</dt> </dl>

 

