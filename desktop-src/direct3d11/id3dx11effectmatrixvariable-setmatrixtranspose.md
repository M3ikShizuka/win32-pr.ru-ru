---
title: Метод ID3DX11EffectMatrixVariable Сетматрикстранспосе (D3dx11effect. h)
description: Переставить и установить матрицу с плавающей точкой.
ms.assetid: 228546c9-0141-4e17-bc8f-bff7201825d7
keywords:
- Метод Сетматрикстранспосе Direct3D 11
- Метод Сетматрикстранспосе Direct3D 11, интерфейс ID3DX11EffectMatrixVariable
- Интерфейс ID3DX11EffectMatrixVariable Direct3D 11, метод Сетматрикстранспосе
topic_type:
- apiref
api_name:
- ID3DX11EffectMatrixVariable.SetMatrixTranspose
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: de86741ba3168276da48756082e2e59f876009523ea940cdb58d070b4e72c3a0
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118535117"
---
# <a name="id3dx11effectmatrixvariablesetmatrixtranspose-method"></a>Метод ID3DX11EffectMatrixVariable:: Сетматрикстранспосе

Переставить и установить матрицу с плавающей точкой.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetMatrixTranspose(
   float *pData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pData* 
</dt> <dd>

Тип: **float \***

Указатель на первый элемент матрицы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращает один из следующих [кодов возврата Direct3D 11](d3d11-graphics-reference-returnvalues.md).

## <a name="remarks"></a>Remarks

При перестановке матрицы порядок данных переупорядочивается из порядка строк в столбец в порядке строк (или наоборот).

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[ID3DX11EffectMatrixVariable](id3dx11effectmatrixvariable.md)
</dt> </dl>

 

 





