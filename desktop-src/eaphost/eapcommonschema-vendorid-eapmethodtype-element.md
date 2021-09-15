---
title: VendorId (Еапмесодтипе), элемент
description: Относится к поставщику, который определил метод, если элемент Type (Еапмесодтипе) имеет значение 254 (Расширенный метод EAP).
ms.assetid: 14992940-2fe5-4f85-91c0-1f61345ee90f
keywords:
- Элемент VendorId EAPHost
topic_type:
- apiref
api_name:
- VendorId
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 9091cdbd7620baf6ec5dc893bd2100b2f04585ec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571867"
---
# <a name="vendorid-eapmethodtype-element"></a>VendorId (Еапмесодтипе), элемент

Элемент **VendorID (еапмесодтипе)** ссылается на поставщика, который определил метод, если элемент [**Type (еапмесодтипе)**](eapcommonschema-type-eapmethodtype-element.md) имеет значение 254 (Расширенный метод EAP).

**ИД поставщика** является необязательным. Если используется, то **ИД поставщика** — это уникальный номер, выданный IANA.

``` syntax
<xs:element name="VendorId"
    type="unsignedInt"
 />
```

Элемент **VendorID** определяется сложным типом [**еапмесодтипе**](eapcommonschema-eapmethodtype-complextype.md) .

## <a name="remarks"></a>Комментарии

Элементы [**аусорид**](eapcommonschema-authorid-eapmethodtype-element.md) и **VendorID** не обязательно должны быть одинаковыми для конкретного метода.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



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

 

 





