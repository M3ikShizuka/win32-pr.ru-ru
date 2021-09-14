---
description: Определяет строковый тип для идентификаторов набора служб (SSID).
ms.assetid: c9e79a3d-7d5c-4320-ade2-40124de00920
title: Простой тип Нетворкнаметипе
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- networkNameType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 6b6463644e1bd174be256d51b34ae2ae4ad9ce07
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147017"
---
# <a name="networknametype-simple-type"></a>Простой тип Нетворкнаметипе

Простой тип Нетворкнаметипе определяет строковый тип для идентификаторов набора служб (SSID). Идентификатор SSID — это строка, которая состоит по крайней мере из одного символа и не длиннее 32 символов.

``` syntax
<xs:simpleType name="networkNameType">
    <xs:restriction
        base="string"
    >
        <xs:minLength
            value="1"
         />
        <xs:maxLength
            value="32"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




