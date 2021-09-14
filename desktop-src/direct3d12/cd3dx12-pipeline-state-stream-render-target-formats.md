---
title: Структура CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS (D3dx12. h)
description: Вспомогательная структура, используемая для описания форматов целевого объекта отрисовки в виде одного объекта, подходящего для описания потока.
ms.assetid: 8C5C2279-7985-41B6-87EA-ABB0007DAFD4
keywords:
- Структура CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS
topic_type:
- apiref
api_name:
- CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS
api_location:
- d3dx12.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5a64f051ba56edf176c87bbc99551cd974fc3a43
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126969850"
---
# <a name="cd3dx12_pipeline_state_stream_render_target_formats-structure"></a>\_ \_ \_ \_ \_ Структура форматов целевого объекта подготовки потока состояния конвейера CD3DX12 \_

Вспомогательная структура, используемая для описания форматов целевого объекта отрисовки в виде одного объекта, подходящего для описания потока.

## <a name="syntax"></a>Синтаксис


```C++
struct CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS {
                                                      CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS;
                                                      CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS(D3D12_RT_FORMAT_ARRAY const &i);
  CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS operator=(D3D12_RT_FORMAT_ARRAY const& i);
                                                      operator D3D12_RT_FORMAT_ARRAY() const;
};
```



## <a name="members"></a>Участники

<dl> <dt>

**\_ \_ \_ \_ \_ Форматы целевого объекта подготовки потока состояния конвейера CD3DX12 \_**
</dt> <dd>

Создает новый, неинициализированный экземпляр \_ потока состояния конвейера CD3DX12, \_ \_ \_ предназначенный для подготовки к просмотру \_ целевых \_ форматов.

</dd> <dt>

**\_ \_ \_ Форматы целевого объекта подготовки потока состояния конвейера CD3DX12 \_ \_ \_ ( \_ \_ \_ константа D3D12 массива формата RT &i)**
</dt> <dd>

Создает новый экземпляр \_ потока состояния конвейера CD3DX12 \_ для \_ \_ подготовки к просмотру \_ целевых форматов \_ , инициализированных с типом подобъекта типа **\_ подобъекта состояния конвейера D3D12, для \_ \_ \_ \_ отображения \_ целевых \_ форматов** и данных подобъектов, скопированных из *i*, структуры [**\_ \_ \_ массива формата D3D12 RT**](/windows/desktop/api/d3d12/ns-d3d12-d3d12_rt_format_array) .

</dd> <dt>

**operator = (D3D12 \_ \_ массива формата RT \_ const& i)**
</dt> <dd>

Оператор присваивания копирования.

</dd> <dt>

**\_ \_ const-оператор D3D12 массив формата RT \_ () константа**
</dt> <dd>

Неявное преобразование в структуру [**\_ \_ \_ массива формата D3D12 RT**](/windows/desktop/api/d3d12/ns-d3d12-d3d12_rt_format_array) .

</dd> </dl>

## <a name="remarks"></a>Комментарии

\_ \_ \_ Форматы целевого объекта подготовки потока состояния конвейера CD3DX12 \_ \_ \_ представляют собой специализацию typedef шаблона [**\_ \_ \_ \_ подобъекта потока состояния конвейера CD3DX12**](cd3dx12-pipeline-state-stream-subobject.md) и определяется следующим образом:


```C++
typedef CD3DX12_PIPELINE_STATE_STREAM_SUBOBJECT<D3D12_RT_FORMAT_ARRAY, D3D12_PIPELINE_STATE_SUBOBJECT_TYPE_RENDER_TARGET_FORMATS>
    CD3DX12_PIPELINE_STATE_STREAM_RENDER_TARGET_FORMATS;
          
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

 

