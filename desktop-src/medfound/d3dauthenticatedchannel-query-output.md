---
description: 'Содержит ответ от метода IDirect3DAuthenticatedChannel9:: Query.'
ms.assetid: b2783b8e-0436-419a-a93e-93dc1b87024d
title: Структура D3DAUTHENTICATEDCHANNEL_QUERY_OUTPUT (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCHANNEL_QUERY_OUTPUT
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: 79fe02a483ade1ff60107287799624017496887b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461016"
---
# <a name="d3dauthenticatedchannel_query_output-structure"></a>\_ \_ Выходная Структура запроса D3DAUTHENTICATEDCHANNEL

Содержит ответ от метода [**IDirect3DAuthenticatedChannel9:: Query**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-query) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _D3DAUTHENTICATEDCHANNEL_QUERY_OUTPUT {
  D3D_OMAC       omac;
  GUID           QueryType;
  hChannel       HANDLE;
  SequenceNumber UINT;
  HRESULT        ReturnCode;
} D3DAUTHENTICATEDCHANNEL_QUERY_OUTPUT;
```



## <a name="members"></a>Участники

<dl> <dt>

**омак**
</dt> <dd>

Структура [**D3D \_ ОМАК**](d3d-omac.md) , содержащая код проверки подлинности сообщения (Mac) данных. Для вычисления этого значения в блоке данных, который отображается после этого элемента структуры, драйвер использует одноключовый CBC MAC (ОМАК) на основе AES.

</dd> <dt>

**QueryType**
</dt> <dd>

Идентификатор GUID, указывающий запрос. Список значений см. в разделе [запросы защита содержимого](content-protection-queries.md).

</dd> <dt>

**СПРАВИТЬСЯ**
</dt> <dd>

Маркер для аутентифицированного канала.

</dd> <dt>

**UINT**
</dt> <dd>

Порядковый номер запроса.

</dd> <dt>

**ReturnCode**
</dt> <dd>

Код результата для запроса.

</dd> </dl>

## <a name="remarks"></a>Remarks

Для членов **QueryType**, **хчаннел** и **SequenceNumber** драйвер использует те же значения, что и приложение, предоставленное в структуре [**\_ \_ входных данных запроса D3DAUTHENTICATEDCHANNEL**](d3dauthenticatedchannel-query-input.md) . Приложение должно проверить, совпадают ли эти значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>D3d9types. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Видеоструктуры Direct3D](direct3d-video-structures.md)
</dt> <dt>

[**IDirect3DAuthenticatedChannel9:: Query**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-query)
</dt> </dl>

 

 




