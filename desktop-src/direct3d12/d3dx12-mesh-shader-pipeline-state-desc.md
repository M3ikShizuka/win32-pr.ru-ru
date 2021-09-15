---
title: Структура D3DX12_MESH_SHADER_PIPELINE_STATE_DESC (D3dx12. h)
description: Для [шейдеров сетки и усиления](https://microsoft.github.io/DirectX-Specs/d3d/MeshShader.html)можно использовать данные из [еффектпипелинестатедескриптион](https://github.com/Microsoft/DirectXTK12/wiki/EffectPipelineStateDescription)с **D3DX12_MESH_SHADER_PIPELINE_STATE_DESC**, чтобы обеспечить все состояние.
keywords:
- Структура D3DX12_MESH_SHADER_PIPELINE_STATE_DESC
topic_type:
- apiref
api_name:
- D3DX12_MESH_SHADER_PIPELINE_STATE_DESC
api_location:
- d3dx12.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 08/02/2021
ms.openlocfilehash: 99ffe747a6cd916f82e3d2ae52f9fa368203da91
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570883"
---
# <a name="d3dx12_mesh_shader_pipeline_state_desc-structure"></a>Структура D3DX12_MESH_SHADER_PIPELINE_STATE_DESC

Для [шейдеров сетки и усиления](https://microsoft.github.io/DirectX-Specs/d3d/MeshShader.html)можно использовать данные из [еффектпипелинестатедескриптион](https://github.com/Microsoft/DirectXTK12/wiki/EffectPipelineStateDescription)с **D3DX12_MESH_SHADER_PIPELINE_STATE_DESC**, чтобы обеспечить все состояние.

См. также [CD3DX12_PIPELINE_STATE_STREAM2](cd3dx12-pipeline-state-stream1.md).

Пример кода см. в разделе [шейдеры сетки](https://github.com/Microsoft/DirectXTK12/wiki/EffectPipelineStateDescription#mesh-shaders).

## <a name="syntax"></a>Синтаксис

```cpp
struct D3DX12_MESH_SHADER_PIPELINE_STATE_DESC
{
    ID3D12RootSignature* pRootSignature;
    D3D12_SHADER_BYTECODE         AS;
    D3D12_SHADER_BYTECODE         MS;
    D3D12_SHADER_BYTECODE         PS;
    D3D12_BLEND_DESC              BlendState;
    UINT                          SampleMask;
    D3D12_RASTERIZER_DESC         RasterizerState;
    D3D12_DEPTH_STENCIL_DESC      DepthStencilState;
    D3D12_PRIMITIVE_TOPOLOGY_TYPE PrimitiveTopologyType;
    UINT                          NumRenderTargets;
    DXGI_FORMAT                   RTVFormats[D3D12_SIMULTANEOUS_RENDER_TARGET_COUNT];
    DXGI_FORMAT                   DSVFormat;
    DXGI_SAMPLE_DESC              SampleDesc;
    UINT                          NodeMask;
    D3D12_CACHED_PIPELINE_STATE   CachedPSO;
    D3D12_PIPELINE_STATE_FLAGS    Flags;
};
```

## <a name="members"></a>Участники

`pRootSignature`

Тип: **[ID3D12RootSignature](/windows/win32/api/d3d12/nn-d3d12-id3d12rootsignature)\***

Объект корневой подписи, определяющий, какие ресурсы привязаны к конвейеру.

`AS`

Тип: **[D3D12_SHADER_BYTECODE](/windows/win32/api/d3d12/ns-d3d12-d3d12_shader_bytecode)**

Содержит данные, представляющие программу шейдера усиления.

`MS`

Тип: **[D3D12_SHADER_BYTECODE](/windows/win32/api/d3d12/ns-d3d12-d3d12_shader_bytecode)**

Содержит данные, представляющие программу шейдера сетки.

`PS`

Тип: **[D3D12_SHADER_BYTECODE](/windows/win32/api/d3d12/ns-d3d12-d3d12_shader_bytecode)**

Содержит данные, представляющие программу шейдера пикселей.

`BlendState`

Тип: **[D3D12_BLEND_DESC](/windows/win32/api/d3d12/ns-d3d12-d3d12_blend_desc)**

Описывает состояние смешения.

`SampleMask`

Тип: **[uint](/windows/win32/winprog/windows-data-types)**

Образец маски для состояния смешения.

`RasterizerState`

Тип: **[D3D12_RASTERIZER_DESC](/windows/win32/api/d3d12/ns-d3d12-d3d12_rasterizer_desc)**

Описывает состояние средства программной прорисовки.

`DepthStencilState`

Тип: **[D3D12_DEPTH_STENCIL_DESC](/windows/win32/api/d3d12/ns-d3d12-d3d12_rasterizer_desc)**

Описывает состояние шаблона глубины.

`PrimitiveTopologyType`

Тип: **[D3D12_PRIMITIVE_TOPOLOGY_TYPE](/windows/win32/api/d3d12/ne-d3d12-d3d12_primitive_topology_type)**

Описывает тип и порядок примитивных данных.

`NumRenderTargets`

Тип: **[uint](/windows/win32/winprog/windows-data-types)**

Число форматов целевого объекта прорисовки в элементе *ртвформатс* .

`RTVFormats`

Тип: **[DXGI_FORMAT](/windows/win32/api/dxgiformat/ne-dxgiformat-dxgi_format)**

Массив значений для форматов целевого объекта прорисовки.

`DSVFormat`

Тип: **[DXGI_FORMAT](/windows/win32/api/dxgiformat/ne-dxgiformat-dxgi_format)**

Значение для формата трафарета глубины.

`SampleDesc`

Тип: **[DXGI_SAMPLE_DESC](/windows/win32/api/dxgiformat/ne-dxgiformat-dxgi_format)**

Задает параметры с множественной выборкой.

`CachedPSO`

Тип: **[D3D12_CACHED_PIPELINE_STATE](/windows/win32/api/d3d12/ns-d3d12-d3d12_cached_pipeline_state)**

Кэшированный объект состояния конвейера. *пкачедблоб* и *качедблобсизеинбитес* могут иметь значение NULL и 0 соответственно.

`Flags`

Тип: **[D3D12_PIPELINE_STATE_FLAGS](/windows/win32/api/d3d12/ne-d3d12-d3d12_pipeline_state_flags)**

Константа перечисления флагов (например, чтобы указать, что состояние конвейера должно быть скомпилировано с дополнительными сведениями для помощи в отладке).

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок | [D3dx12. h](https://github.com/microsoft/DirectX-Headers/blob/main/include/directx/d3dx12.h) |

## <a name="see-also"></a>См. также раздел

* [Вспомогательные структуры для Direct3D 12](helper-structures-for-d3d12.md)
* [CD3DX12_PIPELINE_STATE_STREAM2](cd3dx12-pipeline-state-stream1.md)
* [шейдеры сетки и усиления](https://microsoft.github.io/DirectX-Specs/d3d/MeshShader.html)
* [еффектпипелинестатедескриптион](https://github.com/Microsoft/DirectXTK12/wiki/EffectPipelineStateDescription)
