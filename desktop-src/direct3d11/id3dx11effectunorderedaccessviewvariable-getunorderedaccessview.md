---
title: Метод ID3DX11EffectUnorderedAccessViewVariable Жетунордередакцессвиев (D3dx11effect. h)
description: Получите неупорядоченный доступ к представлению.
ms.assetid: 46f61c4f-b3ee-4058-99b9-a43ca6944fb2
keywords:
- Метод Жетунордередакцессвиев Direct3D 11
- Метод Жетунордередакцессвиев Direct3D 11, интерфейс ID3DX11EffectUnorderedAccessViewVariable
- Интерфейс ID3DX11EffectUnorderedAccessViewVariable Direct3D 11, метод Жетунордередакцессвиев
topic_type:
- apiref
api_name:
- ID3DX11EffectUnorderedAccessViewVariable.GetUnorderedAccessView
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7743d15c2380ff4e38bdcae1d38bbd8905cbccda
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458003"
---
# <a name="id3dx11effectunorderedaccessviewvariablegetunorderedaccessview-method"></a>Метод ID3DX11EffectUnorderedAccessViewVariable:: Жетунордередакцессвиев

Получите неупорядоченный доступ к представлению.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetUnorderedAccessView(
   ID3D11UnorderedAccessView **ppResource
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппресаурце* 
</dt> <dd>

Тип: **[ **ID3D11UnorderedAccessView**](/windows/desktop/api/D3D11/nn-d3d11-id3d11unorderedaccessview)\*\***

Указатель на указатель [**ID3D11UnorderedAccessView**](/windows/desktop/api/D3D11/nn-d3d11-id3d11unorderedaccessview) , который будет установлен при возврате.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращает один из следующих [кодов возврата Direct3D 11](d3d11-graphics-reference-returnvalues.md).

## <a name="remarks"></a>Remarks

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ID3DX11EffectUnorderedAccessViewVariable](id3dx11effectunorderedaccessviewvariable.md)
</dt> </dl>

 

 





