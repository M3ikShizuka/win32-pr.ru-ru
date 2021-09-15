---
title: Вендортипе (Еапмесодтипе), элемент
description: Сведения об элементе Вендортипе (Еапмесодтипе). Этот элемент является типом, определяемым поставщиком для метода.
ms.assetid: baa43e60-05e2-43f9-bb38-896725be76b4
keywords:
- Элемент Вендортипе EAPHost
topic_type:
- apiref
api_name:
- VendorType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 29030672cea0deff59f7f3026dcac98d6ff1c178
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568787"
---
# <a name="vendortype-eapmethodtype-element"></a>Вендортипе (Еапмесодтипе), элемент

Элемент **вендортипе (еапмесодтипе)** является типом, определяемым поставщиком для метода.

Элемент **вендортипе** является необязательным. При использовании **вендортипе** — это уникальный номер, выданный IANA.

``` syntax
<xs:element name="VendorType"
    type="unsignedInt"
 />
```

Элемент **вендортипе** определяется сложным типом [**еапмесодтипе**](eapcommonschema-eapmethodtype-complextype.md) .

## <a name="requirements"></a>Требования



| Роль | Минимальная поддерживаемая версия ОС |
|------|------------------------------|
| Клиент<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Сервер<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**еапмесодтипе**](eapcommonschema-eapmethodtype-complextype.md)
</dt> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема еапкоммон](eapcommonschema-schema.md)
</dt> </dl>

 

 





