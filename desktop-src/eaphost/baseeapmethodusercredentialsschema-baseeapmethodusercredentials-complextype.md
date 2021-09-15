---
title: Сложный тип Басиапмесодусеркредентиалс
description: Сведения о сложном типе Басиапмесодусеркредентиалс. Этот тип является элементом-заполнителем для учетных данных метода.
ms.assetid: ebbf813d-657a-4ff2-acf2-c18ce694b564
keywords:
- Басиапмесодусеркредентиалс сложный тип EAPHost
topic_type:
- apiref
api_name:
- BaseEapMethodUserCredentials
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 37bc7a91a5d90cde6cba1af12bb0a4784ee21c7f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568859"
---
# <a name="baseeapmethodusercredentials-complex-type"></a>Сложный тип Басиапмесодусеркредентиалс

Сложный тип **басиапмесодусеркредентиалс** — это элемент-заполнитель для учетных данных метода.

``` syntax
<xs:complexType name="BaseEapMethodUserCredentials">
    <xs:sequence>
        <xs:any
            processContents="lax"
            minOccurs="0"
            maxOccurs="unbounded"
            namespace="##any"
         />
    </xs:sequence>
</xs:complexType>
```

## <a name="remarks"></a>Remarks

Метод EAP выполняет проверку схемы содержимого **басиапмесодусеркредентиалс**.

## <a name="requirements"></a>Требования



| Роль | Минимальная поддерживаемая версия ОС |
|------|------------------------------|
| Клиент<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Сервер<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема басиапмесодусеркредентиалс](baseeapmethodusercredentialsschema-schema.md)
</dt> </dl>

 

 





