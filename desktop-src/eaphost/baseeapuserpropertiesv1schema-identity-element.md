---
title: Элемент Identity
description: Сведения об элементе удостоверения EAPHost. Этот элемент захватывает удостоверение, используемое для проверки подлинности.
ms.assetid: 464979f0-6a2b-43e7-a207-2fbd1e2e5f51
keywords:
- Элемент Identity EAPHost
topic_type:
- apiref
api_name:
- Identity
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 485d576155d5ac63df2776016f3aafabf8c18c25
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568823"
---
# <a name="identity-element"></a>Элемент Identity

Элемент **Identity** захватывает удостоверение, используемое для проверки подлинности.

``` syntax
<xs:element name="Identity"
    type="string"
 />
```

## <a name="remarks"></a>Remarks

Элемент **Identity** является абстрактным; Каждый метод должен определять и использовать производный элемент в документах экземпляра.

## <a name="requirements"></a>Требования



| Роль | Минимальная поддерживаемая версия ОС |
|------|------------------------------|
| Клиент<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Сервер<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема baseeapuserpropertiesv1](baseeapuserpropertiesv1schema-schema.md)
</dt> </dl>

 

 





