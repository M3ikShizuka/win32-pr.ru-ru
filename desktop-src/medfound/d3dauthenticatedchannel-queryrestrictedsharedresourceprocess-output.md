---
description: Содержит ответ на \_ запрос D3DAUTHENTICATEDQUERY рестриктедшаредресаурцепроцесс.
ms.assetid: 763c56b5-b240-4bad-b601-07959ed37479
title: Структура D3DAUTHENTICATEDCHANNEL_QUERYRESTRICTEDSHAREDRESOURCEPROCESS_OUTPUT (D3d9types. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DAUTHENTICATEDCHANNEL_QUERYRESTRICTEDSHAREDRESOURCEPROCESS_OUTPUT
api_type:
- HeaderDef
api_location:
- d3d9types.h
ms.openlocfilehash: bd93e1cadb7da500a82218924044af79fbb1f493
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461009"
---
# <a name="d3dauthenticatedchannel_queryrestrictedsharedresourceprocess_output-structure"></a>\_ \_ Выходная структура D3DAUTHENTICATEDCHANNEL куерирестриктедшаредресаурцепроцесс

Содержит ответ на запрос [**D3DAUTHENTICATEDQUERY \_ рестриктедшаредресаурцепроцесс**](d3dauthenticatedquery-restrictedsharedresourceprocess.md) .

Чтобы отправить этот запрос, вызовите метод [**IDirect3DAuthenticatedChannel9:: Query**](/windows/desktop/api/d3d9/nf-d3d9-idirect3dauthenticatedchannel9-query).

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _D3DAUTHENTICATEDCHANNEL_QUERYRESTRICTEDSHAREDRESOURCEPROCESS_OUTPUT {
  D3DAUTHENTICATEDCHANNEL_QUERY_OUTPUT          Output;
  UINT                                          ProcessIndex;
  D3DAUTHENTICATEDCHANNEL_PROCESSIDENTIFIERTYPE ProcessIdentifer;
  HANDLE                                        ProcessHandle;
} D3DAUTHENTICATEDCHANNEL_QUERYRESTRICTEDSHAREDRESOURCEPROCESS_OUTPUT;
```



## <a name="members"></a>Участники

<dl> <dt>

**Выходные данные**
</dt> <dd>

[**\_ \_ Выходная Структура запроса D3DAUTHENTICATEDCHANNEL**](d3dauthenticatedchannel-query-output.md) , которая содержит код проверки подлинности сообщения (Mac) и другие данные.

</dd> <dt>

**процессиндекс**
</dt> <dd>

Индекс процесса в списке процессов.

</dd> <dt>

**процессидентифер**
</dt> <dd>

Значение [**D3DAUTHENTICATEDCHANNEL \_ процессидентифиертипе**](d3dauthenticatedchannel-processidentifiertype.md) , указывающее тип процесса.

</dd> <dt>

**процесшандле**
</dt> <dd>

Обработчик процесса. Если элемент **процессидентифиер** равен **процессидтипе \_ Handle**, то элемент **процесшандле** содержит допустимый обработчик для процесса. В противном случае этот элемент игнорируется.

</dd> </dl>

## <a name="remarks"></a>Remarks

Процесс диспетчер окон рабочего стола (DWM) определяется путем установки **процессидентифиер** равным **процессидтипе \_ DWM**. Другие процессы определяются путем установки обработчика процесса в **процесшандле** и установки **Процессидентифиер** равным **процессидтипе \_ Handle**.

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

 

 




