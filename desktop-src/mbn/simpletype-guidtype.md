---
description: Строковое представление GUID в обычном формате.
MS-HAID: WWAN\_profile\_v4.simpleType\_guidType
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: простой тип Гуидтипе (мобильное широкополосное подключение)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 66b7cc19207ab334694e4b42a49f727070cb385d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469315"
---
# <a name="span-idwwan_profile_v4simpletype_guidtypespanguidtype-simple-type-mobile-broadband"></a><span id="WWAN_profile_v4.simpleType_guidType"></span>простой тип Гуидтипе (мобильное широкополосное подключение)

Строковое представление GUID в обычном формате.

``` syntax
<xs:simpleType name="guidType">
    <xs:restriction
        base="token"
    >
        <xs:pattern
            value="{[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}}"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="patterns"></a>Шаблоны

Простой тип **гуидтипе** — это токен, который ограничен следующим шаблоном:

-   `{[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}}`

 

 



