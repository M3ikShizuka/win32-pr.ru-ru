---
title: Connections, элемент
description: Сведения об элементе Connections. Этот элемент собирает и содержит ноль или более элементов соединения.
ms.assetid: 2c199338-892f-4d8c-bf33-4a19f362de3e
keywords:
- Элемент Connections EAPHost
topic_type:
- apiref
api_name:
- Connections
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 6cdb23c9f1a6130e2fe77061286e8a0657c3e2f5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568786"
---
# <a name="connections-element"></a>Connections, элемент

Элемент **Connections** собирает и содержит ноль или более элементов [**соединения**](eapconnectionpropertiesv1schema-connection-connections-element.md) .

``` syntax
<xs:element name="Connections">
    <xs:complexType>
        <xs:sequence>
            <xs:element name="Connection"
                minOccurs="0"
                maxOccurs="unbounded"
            >
                <xs:complexType>
                    <xs:sequence>
                        <xs:element name="Name"
                            type="string"
                         />
                        <xs:element
                            maxOccurs="unbounded"
                            ref="Eap"
                         />
                    </xs:sequence>
                </xs:complexType>
            </xs:element>
        </xs:sequence>
    </xs:complexType>
</xs:element>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                              | Тип   | Описание                                                                                                                                                                                |
|--------------------------------------------------------------------------------------|--------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Протокола**](baseeapconnectionpropertiesv1schema-eap-element.md)                       |        | Определяет элемент конфигурации EAP.<br/>                                                                                                                                       |
| [**Соединение**](eapconnectionpropertiesv1schema-connection-connections-element.md) |        | Определяет каждый параметр конфигурации и связывает его с именем. Элемент [**Connection**](eapconnectionpropertiesv1schema-connection-connections-element.md) является необязательным.<br/> |
| [**Безымян**](eapconnectionpropertiesv1schema-name-connection-element.md)              | строка | Захватывает имя определяемого соединения, помогая идентифицировать несколько соединений.<br/>                                                                     |



## <a name="remarks"></a>Remarks

Элемент **Connections** не используется с устаревшими методами через API-интерфейсы EAPHost.

## <a name="requirements"></a>Требования



| Роль | Минимальная поддерживаемая версия ОС |
|------|------------------------------|
| Клиент<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Сервер<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема eapconnectionpropertiesv1](eapconnectionpropertiesv1schema-schema.md)
</dt> </dl>

 

 





