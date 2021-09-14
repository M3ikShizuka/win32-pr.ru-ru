---
title: Структура CD3DX12_PIPELINE_STATE_STREAM_FLAGS (D3dx12. h)
description: Вспомогательная структура, используемая для описания флагов состояния конвейера в виде одного объекта, подходящего для описания потока.
ms.assetid: EF67936B-315A-4B3F-9E07-7CF4C5EE47CF
keywords:
- Структура CD3DX12_PIPELINE_STATE_STREAM_FLAGS
topic_type:
- apiref
api_name:
- CD3DX12_PIPELINE_STATE_STREAM_FLAGS
api_location:
- d3dx12.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 034f4a63c774ca41f28fbe9e6c2945fddee47c4f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126969886"
---
# <a name="cd3dx12_pipeline_state_stream_flags-structure"></a>\_ \_ \_ \_ Структура флагов потока состояния конвейера CD3DX12

Вспомогательная структура, используемая для описания флагов состояния конвейера в виде одного объекта, подходящего для описания потока.

## <a name="syntax"></a>Синтаксис


```C++
struct CD3DX12_PIPELINE_STATE_STREAM_FLAGS {
                                      CD3DX12_PIPELINE_STATE_STREAM_FLAGS;
                                      CD3DX12_PIPELINE_STATE_STREAM_FLAGS(D3D12_PIPELINE_STATE_FLAGS const &i);
  CD3DX12_PIPELINE_STATE_STREAM_FLAGS operator=(D3D12_PIPELINE_STATE_FLAGS const& i);
                                      operator D3D12_PIPELINE_STATE_FLAGS() const;
};
```



## <a name="members"></a>Участники

<dl> <dt>

**\_ \_ \_ Флаги потока состояния конвейера CD3DX12 \_**
</dt> <dd>

Создает новый, неинициализированный экземпляр \_ \_ \_ флагов потока состояния конвейера CD3DX12 \_ .

</dd> <dt>

**\_ \_ Флаги потока состояния конвейера CD3DX12 \_ \_ ( \_ \_ флаги состояния конвейера D3D12 \_ const &i)**
</dt> <dd>

Создает новый экземпляр \_ \_ флагов потока состояния конвейера \_ CD3DX12 \_ , которые инициализируются с типом подобъекта **\_ \_ \_ \_ \_ флагов типа подобъекта состояния конвейера D3D12** и данными подобъектов, скопированными из *i*, структурой [**\_ \_ \_ флагов состояния конвейера D3D12**](/windows/desktop/api/d3d12/ne-d3d12-d3d12_pipeline_state_flags) .

</dd> <dt>

**operator = (D3D12 \_ \_ флаги состояния конвейера \_ "const"& i)**
</dt> <dd>

Оператор присваивания копирования.

</dd> <dt>

**\_флаг состояния конвейера оператора D3D12 \_ \_ () const**
</dt> <dd>

Неявное преобразование в структуру [**\_ \_ \_ флагов состояния конвейера D3D12**](/windows/desktop/api/d3d12/ne-d3d12-d3d12_pipeline_state_flags) .

</dd> </dl>

## <a name="remarks"></a>Комментарии

\_ \_ Флаги потока состояния конвейера CD3DX12 \_ \_ являются специализацией typedef [**шаблона \_ \_ \_ \_ подобъекта потока состояния конвейера CD3DX12**](cd3dx12-pipeline-state-stream-subobject.md) и определяются следующим образом:


```C++
typedef CD3DX12_PIPELINE_STATE_STREAM_SUBOBJECT<D3D12_PIPELINE_STATE_FLAGS, D3D12_PIPELINE_STATE_SUBOBJECT_TYPE_FLAGS>
    CD3DX12_PIPELINE_STATE_STREAM_FLAGS;
          
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

 

