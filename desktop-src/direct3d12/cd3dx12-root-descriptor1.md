---
title: Структура CD3DX12_ROOT_DESCRIPTOR1 (D3dx12. h)
description: Вспомогательная структура, позволяющая легко инициализировать D3D12 \_ корневую \_ структуру DESCRIPTOR1.
ms.assetid: 664822BF-5C27-4541-953F-219894547A6C
keywords:
- Структура CD3DX12_ROOT_DESCRIPTOR1
topic_type:
- apiref
api_name:
- CD3DX12_ROOT_DESCRIPTOR1
api_location:
- d3dx12.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e75fd8274e9f1901274c8002a6826b4c7633b3afae78d10ad9be2abad7d74ecf
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120028234"
---
# <a name="cd3dx12_root_descriptor1-structure"></a>CD3DX12 \_ корневая \_ Структура DESCRIPTOR1

Вспомогательная структура, позволяющая легко инициализировать [**D3D12 \_ корневую структуру \_ DESCRIPTOR1**](/windows/desktop/api/d3d12/ns-d3d12-d3d12_root_descriptor1) .

## <a name="syntax"></a>Синтаксис


```C++
struct CD3DX12_ROOT_DESCRIPTOR1  : public D3D12_ROOT_DESCRIPTOR1{
       CD3DX12_ROOT_DESCRIPTOR1();
       explicit CD3DX12_ROOT_DESCRIPTOR1(const D3D12_ROOT_DESCRIPTOR1 &o);
       CD3DX12_ROOT_DESCRIPTOR1(UINT shaderRegister, UINT registerSpace = 0, D3D12_ROOT_DESCRIPTOR_FLAGS flags = D3D12_ROOT_DESCRIPTOR_FLAG_NONE);
  void inline Init(UINT shaderRegister, UINT registerSpace = 0, D3D12_ROOT_DESCRIPTOR_FLAGS flags = D3D12_ROOT_DESCRIPTOR_FLAG_NONE);
  void static inline Init(D3D12_ROOT_DESCRIPTOR1 &table, UINT shaderRegister, UINT registerSpace = 0, D3D12_ROOT_DESCRIPTOR_FLAGS flags = D3D12_ROOT_DESCRIPTOR_FLAG_NONE);
};
```



## <a name="members"></a>Члены

<dl> <dt>

**CD3DX12 \_ root \_ DESCRIPTOR1 ()**
</dt> <dd>

Создает новый, неинициализированный экземпляр экземпляра CD3DX12 \_ root \_ DESCRIPTOR1.

</dd> <dt>

**явное CD3DX12 \_ корневой \_ DESCRIPTOR1 (const D3D12 \_ root \_ DESCRIPTOR1 &o)**
</dt> <dd>

Создает новый экземпляр CD3DX12 \_ root \_ DESCRIPTOR1, который инициализируется с содержимым другой [**D3D12 \_ корневой структуры \_ DESCRIPTOR1**](/windows/desktop/api/d3d12/ns-d3d12-d3d12_root_descriptor1) .

</dd> <dt>

**CD3DX12 \_ root \_ DESCRIPTOR1 (uint ШАДЕРРЕГИСТЕР, uint регистерспаце = 0, D3D12 флаги \_ \_ \_ flags root-дескриптора = D3D12 \_ корневой \_ \_ флага \_ None)**
</dt> <dd>

Создает новый экземпляр CD3DX12 \_ root \_ DESCRIPTOR1, инициализируя следующие параметры:

UINT Шадеррегистер

UINT Регистерспаце = 0

[**D3D12 \_ Флаги флагов КОРНЕВого \_ дескриптора \_**](/windows/desktop/api/d3d12/ne-d3d12-d3d12_root_descriptor_flags) = D3D12 \_ корневого \_ дескриптора \_ \_ None

</dd> <dt>

**Inline init (UINT Шадеррегистер, UINT Регистерспаце = 0, D3D12 flags \_ root \_ дескриптора флаг \_ = D3D12 \_ корневого \_ дескриптора \_ \_ None)**
</dt> <dd>

Задает функцию, которая инициализирует следующие параметры:

UINT Шадеррегистер

UINT Регистерспаце = 0

[**D3D12 \_ Флаги флагов КОРНЕВого \_ дескриптора \_**](/windows/desktop/api/d3d12/ne-d3d12-d3d12_root_descriptor_flags) = D3D12 \_ корневого \_ дескриптора \_ \_ None

</dd> <dt>

**Статическая встроенная инициализация (D3D12 \_ root \_ DESCRIPTOR1 &таблица, uint ШАДЕРРЕГИСТЕР, uint регистерспаце = 0, D3D12 флаги \_ \_ битового дескриптора [- \_ D3D12 \_ корневого \_ дескриптора \_ \_ None)**
</dt> <dd>

Задает функцию, которая инициализирует следующие параметры:

[**D3D12 \_ Корневая \_ DESCRIPTOR1**](/windows/desktop/api/d3d12/ns-d3d12-d3d12_root_descriptor1) &таблица

UINT Шадеррегистер

UINT Регистерспаце = 0

[**D3D12 \_ Флаги флагов КОРНЕВого \_ дескриптора \_**](/windows/desktop/api/d3d12/ne-d3d12-d3d12_root_descriptor_flags) = D3D12 \_ корневого \_ дескриптора \_ \_ None

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx12. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_Корневой \_ DESCRIPTOR1 D3D12**](/windows/desktop/api/d3d12/ns-d3d12-d3d12_root_descriptor1)
</dt> <dt>

[Вспомогательные структуры для D3D12](helper-structures-for-d3d12.md)
</dt> </dl>

 

 





