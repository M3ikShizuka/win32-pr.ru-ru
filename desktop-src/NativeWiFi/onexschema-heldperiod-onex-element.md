---
description: Указывает период времени в секундах, в течение которого клиент не будет повторно пытаться пройти проверку подлинности после неудачной попытки проверки подлинности.
ms.assetid: a6b32e88-da36-4aea-a01d-f5f7bc37d171
title: Элемент Хелдпериод (OneX)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- heldPeriod
api_type:
- Schema
api_location: ''
ms.openlocfilehash: f8664543a9ea5b0f3b290168129e589e9ccd68ab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127169444"
---
# <a name="heldperiod-onex-element"></a>Элемент Хелдпериод (OneX)

Элемент Хелдпериод (OneX) указывает продолжительность времени в секундах, в течение которого клиент не будет повторно пытаться пройти проверку подлинности после неудачной попытки проверки подлинности.

Этот элемент является необязательным. Если Хелдпериод не указан в профиле, используется значение, равное 1 секунде.

**Windows XP с SP3 и API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2):** Этот элемент будет пропущен, если он есть в профиле.

``` syntax
<xs:element name="heldPeriod">
    <xs:simpleType>
        <xs:restriction
            base="integer"
        >
            <xs:enumeration
                value="1"
             />
            <xs:enumeration
                value="3600"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент **хелдпериод** определяется элементом [**OneX**](onexschema-onex-element.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**Таймаут**](onexschema-onex-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Таймаут**](onexschema-onex-element.md)
</dt> </dl>

 

 




