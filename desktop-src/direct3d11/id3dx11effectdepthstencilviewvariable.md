---
title: Интерфейс ID3DX11EffectDepthStencilViewVariable (D3dx11effect. h)
description: Интерфейс "Глубина-трафарет-представление-переменная" обращается к представлению трафарета глубины.
ms.assetid: 316bf0cc-a7cd-4a40-932a-d566e3c2001e
keywords:
- Интерфейс ID3DX11EffectDepthStencilViewVariable Direct3D 11
- Интерфейс ID3DX11EffectDepthStencilViewVariable Direct3D 11, описание
topic_type:
- apiref
api_name:
- ID3DX11EffectDepthStencilViewVariable
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 51961bd1300157eef4acb4dd15484d5146a166f7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126963817"
---
# <a name="id3dx11effectdepthstencilviewvariable-interface"></a>Интерфейс ID3DX11EffectDepthStencilViewVariable

Интерфейс "Глубина-трафарет-представление-переменная" обращается к представлению трафарета глубины.

## <a name="members"></a>Элементы

Интерфейс **ID3DX11EffectDepthStencilViewVariable** наследует от [**ID3DX11EffectVariable**](id3dx11effectvariable.md). **ID3DX11EffectDepthStencilViewVariable** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **ID3DX11EffectDepthStencilViewVariable** содержит следующие методы.



| Метод                                                                                     | Описание                                              |
|:-------------------------------------------------------------------------------------------|:---------------------------------------------------------|
| [**жетдепсстенЦил**](id3dx11effectdepthstencilviewvariable-getdepthstencil.md)           | Получите ресурс представления глубины-трафаретов.<br/>            |
| [**жетдепсстенЦиларрай**](id3dx11effectdepthstencilviewvariable-getdepthstencilarray.md) | Получите массив ресурсов представления глубины набора элементов.<br/> |
| [**сетдепсстенЦил**](id3dx11effectdepthstencilviewvariable-setdepthstencil.md)           | Задайте ресурс представления глубины-набор.<br/>            |
| [**сетдепсстенЦиларрай**](id3dx11effectdepthstencilviewvariable-setdepthstencilarray.md) | Установите массив ресурсов представления глубины набора элементов.<br/> |



 

## <a name="remarks"></a>Комментарии

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ID3DX11EffectVariable**](id3dx11effectvariable.md)
</dt> <dt>

[Effects 11, интерфейсы](d3d11-graphics-reference-effects11-interfaces.md)
</dt> <dt>

[Интерфейсы D3DX](d3d11-graphics-reference-d3dx11-interfaces.md)
</dt> </dl>

 

 





