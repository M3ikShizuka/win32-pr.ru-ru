---
description: указывает, отображаются ли запрещенные сети в мастере Подключение сети.
ms.assetid: d0a13a80-2532-4383-8946-2536cc1f5e12
title: Шовдениеднетворк (Глобалфлагс), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- showDeniedNetwork
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 33049dad00e5fda22e3f739d3dc200a282481a8f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146993"
---
# <a name="showdeniednetwork-globalflags-element"></a>Шовдениеднетворк (Глобалфлагс), элемент

элемент **шовдениеднетворк** (глобалфлагс) указывает, отображаются ли запрещенные сети в мастере **Подключение к сети** . Сети могут быть отклонены групповой политикой или параметрами пользователя. если **шовдениеднетворк** имеет значение TRUE, в мастере **Подключение к сети** отображаются запрещенные сети. в противном случае запрещенные сети не будут отображаться в мастере.

Этот элемент обязателен. При создании профиля службой автонастройки этот элемент будет принимать значение по умолчанию FALSE.

``` syntax
<xs:element name="showDeniedNetwork"
    type="boolean"
 />
```

Элемент **шовдениеднетворк** определяется элементом [**глобалфлагс**](wlan-policyschema-globalflags-wlanpolicy-element.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**глобалфлагс**](wlan-policyschema-globalflags-wlanpolicy-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Глобалфлагс (Вланполици)**](wlan-policyschema-globalflags-wlanpolicy-element.md)
</dt> </dl>

 

 




