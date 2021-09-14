---
title: Структура CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT (D3dx12. h)
description: Вспомогательная структура, используемая для описания формата трафарета глубины в виде одного объекта, подходящего для описания потока.
ms.assetid: 512DB46E-D8F0-482B-9174-C786FB91AFD2
keywords:
- Структура CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT
topic_type:
- apiref
api_name:
- CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT
api_location:
- d3dx12.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8dc7ae2703ac80ac155c04d42624a081723288bf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126969898"
---
# <a name="cd3dx12_pipeline_state_stream_depth_stencil_format-structure"></a>\_ \_ \_ \_ \_ Структура формата трафарета глубины потока состояния конвейера CD3DX12 \_

Вспомогательная структура, используемая для описания формата трафарета глубины в виде одного объекта, подходящего для описания потока.

## <a name="syntax"></a>Синтаксис


```C++
struct CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT {
                                                     CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT;
                                                     CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT(DXGI_FORMAT const &i);
  CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT operator=(DXGI_FORMAT const& i);
                                                     operator DXGI_FORMAT() const;
};
```



## <a name="members"></a>Участники

<dl> <dt>

**\_ \_ \_ \_ \_ Формат трафарета глубины потока состояния конвейера CD3DX12 \_**
</dt> <dd>

Создает новый, неинициализированный экземпляр \_ \_ \_ \_ \_ формата трафарета глубины потока состояния конвейера CD3DX12 \_ .

</dd> <dt>

**\_ \_ \_ Формат трафарета глубины потока состояния конвейера CD3DX12 \_ \_ \_ ( \_ константа формата DXGI const &i)**
</dt> <dd>

Создает новый экземпляр \_ \_ \_ формата трафарета глубины потока состояния конвейера CD3DX12 \_ \_ \_ , инициализированного с типом подобъекта типа **\_ \_ подобъекта состояния конвейера D3D12 \_ \_ \_ \_ \_ Формат трафарета глубины** и данные подобъекта, скопированные из *i*, перечисление в [**\_ формате DXGI**](/windows/desktop/api/dxgiformat/ne-dxgiformat-dxgi_format) .

</dd> <dt>

**operator = ( \_ константа формата DXGI& i)**
</dt> <dd>

Оператор присваивания копирования.

</dd> <dt>

**Оператор \_ Format DXGI () const**
</dt> <dd>

Неявное преобразование в перечисление [**\_ формата DXGI**](/windows/desktop/api/dxgiformat/ne-dxgiformat-dxgi_format) .

</dd> </dl>

## <a name="remarks"></a>Комментарии

\_ \_ \_ Формат трафарета глубины потока состояния конвейера CD3DX12 \_ \_ \_ является специализацией typedef [**шаблона \_ \_ \_ \_ подобъекта потока состояния конвейера CD3DX12**](cd3dx12-pipeline-state-stream-subobject.md) и определяется следующим образом:


```C++
typedef CD3DX12_PIPELINE_STATE_STREAM_SUBOBJECT<DXGI_FORMAT, D3D12_PIPELINE_STATE_SUBOBJECT_TYPE_DEPTH_STENCIL_FORMAT>
    CD3DX12_PIPELINE_STATE_STREAM_DEPTH_STENCIL_FORMAT;
          
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx12. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Вспомогательные структуры для D3D12](helper-structures-for-d3d12.md)
</dt> <dt>

[**\_Подобъект \_ потока состояния КОНВЕЙЕРа CD3DX12 \_ \_**](cd3dx12-pipeline-state-stream-subobject.md)
</dt> <dt>

[**\_ \_ \_ Тип подобъекта состояния конвейера D3D12 \_**](/windows/desktop/api/d3d12/ne-d3d12-d3d12_pipeline_state_subobject_type)
</dt> </dl>

 

