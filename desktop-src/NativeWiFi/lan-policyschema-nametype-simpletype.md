---
description: Определяет строковый тип для имени или описания профиля политики проводной локальной сети.
ms.assetid: 89de1e7a-618d-4501-a134-c7a37f9c552d
title: простой тип Наметипе (LAN_policy)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- nameType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 702ee6340fa3d03217c884a48625d3a38be4ad9c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065047"
---
# <a name="nametype-simple-type-lan_policy"></a>простой тип Наметипе (LAN_policy)

Простой тип Наметипе определяет строковый тип для имени или описания профиля политики проводной локальной сети. Имена и описания — это строки длиной не менее одного символа и не более 255 символов.

``` syntax
<xs:simpleType name="nameType">
    <xs:restriction
        base="string"
    >
        <xs:minLength
            value="1"
         />
        <xs:maxLength
            value="255"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




