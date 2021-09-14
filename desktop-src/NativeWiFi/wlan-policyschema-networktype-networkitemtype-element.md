---
description: Указывает тип сети.
ms.assetid: fe3044ab-6e93-48f8-b8cb-fdf984987232
title: Нетворктипе (Нетворкитемтипе), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- networkType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: c63b8afdaf699fde6871c198a8235772c59da1ee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147014"
---
# <a name="networktype-networkitemtype-element"></a>Нетворктипе (Нетворкитемтипе), элемент

Элемент Нетворктипе (Нетворкитемтипе) указывает тип сети. Существует два типа сетей: сети инфраструктуры (ESS) и ad-hoc Network (ИБСС).

``` syntax
<xs:element name="networkType"
    type="networkTypeType"
 />
```

Элемент **нетворктипе** определяется сложным типом [**нетворкитемтипе**](wlan-policyschema-networkitemtype-complextype.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**нетворкитемтипе**](wlan-policyschema-networkitemtype-complextype.md)
</dt> <dt>

**Возможные непосредственные родительские элементы в экземпляре схемы**
</dt> <dt>

[**сеть (разрешенных)**](wlan-policyschema-network-allowlist-element.md)
</dt> <dt>

[**сеть (списка блокировки)**](wlan-policyschema-network-blocklist-element.md)
</dt> </dl>

 

 




