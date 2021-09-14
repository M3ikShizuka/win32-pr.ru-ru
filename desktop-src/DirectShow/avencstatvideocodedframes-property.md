---
description: Возвращает число закодированных видеокадров.
ms.assetid: ade9fe69-b3dd-44aa-856b-75d4a7e4c680
title: Свойство Авенкстатвидеокодедфрамес (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3aed3ed0a06003807a6bd0db90b8978282042daf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127148273"
---
# <a name="avencstatvideocodedframes-property"></a>Авенкстатвидеокодедфрамес, свойство

Возвращает число закодированных видеокадров.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенкстатвидеокодедфрамес**

## <a name="remarks"></a>Remarks

Это свойство доступно после завершения кодирования.

Значение этого свойства равно значению свойства [**авенкстатвидеототалфрамес**](avencstatvideototalframes-property.md) минус число пропущенных кадров. Кодировщик может удалить кадры, чтобы остаться в заданных ограничениях скорости. Он также может удалять кадры в конце потока (см. свойство [**авенккоммонстреамендхандлинг**](avenccommonstreamendhandling-property.md) ).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional приложения \[ UWP для классических приложений \|\]<br/>                     |
| Минимальная версия сервера<br/> | \[приложения UWP для классических приложений Windows 2000 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства кодека API](codec-api-properties.md)
</dt> <dt>

[**Интерфейс Икодекапи**](/windows/desktop/api/Strmif/nn-strmif-icodecapi)
</dt> </dl>

 

 




