---
title: Элемент Еаптипе (свойство соединения со схемой v1)
description: Сведения об элементе Еаптипе. Этот элемент захватывает конфигурацию, зависящую от метода, внутри элемента EAP. | Элемент Еаптипе (свойство соединения со схемой v1)
ms.assetid: f953e150-64cf-41b2-937f-410799be4602
keywords:
- Элемент Еаптипе EAPHost
topic_type:
- apiref
api_name:
- EapType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 88361931946f8a209c5b1c41bd17fcbd0e44096d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241309"
---
# <a name="eaptype-element-v1-schema-connection-property"></a>Элемент Еаптипе (свойство соединения со схемой v1)

Элемент **еаптипе** фиксирует конфигурацию, относящуюся к методу, внутри элемента EAP.

``` syntax
<xs:element name="EapType"
    type="BaseEapTypeParameters"
 />
```

## <a name="remarks"></a>Remarks

Элемент **еаптипе** является абстрактным; Каждый метод должен определять и использовать производный элемент в документах экземпляра.

## <a name="requirements"></a>Требования



| Роль | Минимальная поддерживаемая версия ОС |
|------|------------------------------|
| Клиент<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Сервер<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема baseeapconnectionpropertiesv1](baseeapconnectionpropertiesv1schema-schema.md)
</dt> </dl>

 

 





