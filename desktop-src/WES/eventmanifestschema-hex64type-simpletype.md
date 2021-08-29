---
title: Простой тип HexInt64Type
description: Определяет 8-байтовый шестнадцатеричный тип. | Простой тип HexInt64Type
ms.assetid: 2e81ec2b-cf67-42df-92a0-bf45b6dca051
keywords:
- Журнал событий простого типа HexInt64Type
topic_type:
- apiref
api_name:
- HexInt64Type
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 22b0cacc482f5bde657c9cf5eb451acb273e79cda0cbf14a4d3536fe90af756c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119652424"
---
# <a name="hexint64type-simple-type"></a>Простой тип HexInt64Type

Определяет 8-байтовый шестнадцатеричный тип.

``` syntax
<xs:simpleType name="HexInt64Type">
    <xs:restriction
        base="string"
    >
        <xs:pattern
            value="0[xX][0-9A-Fa-f]{1,16}"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="patterns"></a>Шаблоны

Простой тип **HexInt64Type** — это [строка](/dotnet/api/system.string) , которая ограничена следующим шаблоном:

-   `0[xX][0-9A-Fa-f]{1,16}`

    Значение может содержать от одного до шестнадцати шестнадцатеричных символов (например, 0xA или 0xac7bd361004fe190).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

