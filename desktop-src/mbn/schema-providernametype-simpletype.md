---
description: Определяет строковый тип для элемента ProviderName в профиле мобильного широкополосного подключения.
ms.assetid: 1644ded2-f931-4920-848d-e0405d8723e3
title: Простой тип Провидернаметипе
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- providerNameType
api_type:
- Schema
ms.openlocfilehash: df61473358a9ed4453bc28f1b5c7974082e515bb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252553"
---
# <a name="providernametype-simple-type"></a>Простой тип Провидернаметипе

Простой тип **провидернаметипе** определяет строковый тип для элемента [**providerName**](schema-providername-providertype-element.md) в профиле мобильного широкополосного подключения. Эта строка состоит по меньшей мере из одного символа и не длиннее 20 символов.

``` syntax
<xs:simpleType name="providerNameType">
    <xs:restriction
        base="normalizedString"
    >
        <xs:minLength
            value="1"
         />
        <xs:maxLength
            value="20"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                         |



 

 




