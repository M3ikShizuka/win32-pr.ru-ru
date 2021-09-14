---
title: Метод ID3DX11Effect Жетконстантбуффербинаме (D3dx11effect. h)
description: Получение буфера констант по имени.
ms.assetid: 11757615-4068-430d-9ab0-f83f02af8e55
keywords:
- Метод Жетконстантбуффербинаме Direct3D 11
- Метод Жетконстантбуффербинаме Direct3D 11, интерфейс ID3DX11Effect
- Интерфейс ID3DX11Effect Direct3D 11, метод Жетконстантбуффербинаме
topic_type:
- apiref
api_name:
- ID3DX11Effect.GetConstantBufferByName
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fa01d20bfeebfa3f689a58aae5c5face8b879e3c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056039"
---
# <a name="id3dx11effectgetconstantbufferbyname-method"></a>Метод ID3DX11Effect:: Жетконстантбуффербинаме

Получение буфера констант по имени.

## <a name="syntax"></a>Синтаксис


```C++
ID3DX11EffectConstantBuffer* GetConstantBufferByName(
   LPCSTR Name
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*имя*; 
</dt> <dd>

Тип: **[ **LPCSTR**](/windows/desktop/WinProg/windows-data-types)**

Имя константного буфера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **ID3DX11EffectConstantBuffer**](id3dx11effectconstantbuffer.md)\***

Указатель на буфер константы, указанный в имени. См. [**ID3DX11EffectConstantBuffer**](id3dx11effectconstantbuffer.md).

## <a name="remarks"></a>Комментарии

Для действия, содержащего переменную, которая будет доступна для чтения и записи приложением, требуется по крайней мере один буфер константы. Для лучшей производительности результат должен организовывать переменные в один или несколько буферов констант в зависимости от частоты обновления.

> [!Note]  
> Пакет SDK для DirectX не предоставляет никаких скомпилированных двоичных файлов для эффектов. Для создания приложения типа Effects необходимо использовать исходный текст Effects 11. Дополнительные сведения об использовании источника Effects 11 см. в разделе [различия между эффектами 10 и эффекты 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx11effect. h</dt> </dl>                                                    |
| Библиотека<br/> | <dl> <dt>Н/д (библиотека Effects 11 доступна в сети в качестве общего источника.)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[ID3DX11Effect](id3dx11effect.md)
</dt> </dl>

 

