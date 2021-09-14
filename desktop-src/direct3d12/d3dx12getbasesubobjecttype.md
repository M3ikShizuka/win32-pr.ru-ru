---
title: Функция D3DX12GetBaseSubobjectType (D3dx12. h)
description: Возвращает тип подобъекта, соответствующий базовому классу переданного типа подобъекта.
ms.assetid: 3744B042-094C-4EA4-8185-A018B728D843
keywords:
- Функция D3DX12GetBaseSubobjectType
topic_type:
- apiref
api_name:
- D3DX12GetBaseSubobjectType
api_location:
- D3D12.dll
api_type:
- DllExport
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0b39f1c61be682d55512772bef1258aecdb009a5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343883"
---
# <a name="d3dx12getbasesubobjecttype-function"></a>Функция D3DX12GetBaseSubobjectType

Возвращает тип подобъекта, соответствующий базовому классу переданного типа подобъекта.

## <a name="syntax"></a>Синтаксис


```C++
D3D12_PIPELINE_STATE_SUBOBJECT_TYPE inline D3DX12GetBaseSubobjectType(
   D3D12_PIPELINE_STATE_SUBOBJECT_TYPE SubobjectType
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*субобжекттипе* 
</dt> <dd>

Тип: **\_ \_ \_ \_ тип подобъекта состояния конвейера D3D12**

Значение перечисления, указывающее тип подобъекта, который вас интересует.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **\_ \_ \_ \_ тип подобъекта состояния конвейера D3D12**

Если *субобжекттипе* соответствует типу данных подобъекта, производного от другого типа данных подобъекта, возвращается тип подобъекта базового типа данных подобъекта. в противном случае возвращается переданный тип подобъекта. Например, если передается **\_ \_ \_ \_ \_ глубина \_ STENCIL1 типа вложенного объекта состояния конвейера D3D12** , то возвращается **\_ \_ \_ \_ \_ \_ набор элементов с типом подобъекта глубины конвейера D3D12** .

## <a name="remarks"></a>Remarks

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3dx12. h</dt> </dl>  |
| Библиотека<br/> | <dl> <dt>D3D12. lib</dt> </dl> |
| DLL<br/>     | <dl> <dt>D3D12.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Вспомогательные функции для D3D12](helper-functions-for-d3d12.md)
</dt> </dl>

 

 





