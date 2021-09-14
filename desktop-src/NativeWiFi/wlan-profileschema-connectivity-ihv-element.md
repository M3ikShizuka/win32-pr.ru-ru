---
description: Содержит параметры подключения, связанные с IHV. В настоящее время он не реализован.
ms.assetid: d943e82a-8660-4df7-8f5c-42ed83f17313
title: Элемент подключения (IHV)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- connectivity
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 257addbcbd721e5930405e3954dcb348f367af93
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127245539"
---
# <a name="connectivity-ihv-element"></a>Элемент подключения (IHV)

Элемент подключения (IHV) содержит параметры подключения, связанные с IHV. В настоящее время он не реализован.

**Windows XP с SP3 и API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2):** Этот элемент не поддерживается.

``` syntax
<xs:element name="connectivity"
    minOccurs="0"
>
    <xs:complexType>
        <xs:sequence>
            <xs:any
                processContents="lax"
                namespace="##other"
             />
        </xs:sequence>
    </xs:complexType>
</xs:element>
```

Элемент определяется элементом [**IHV**](wlan-profileschema-ihv-wlanprofile-element.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**АППАРАТ**](wlan-profileschema-ihv-wlanprofile-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**IHV (Вланпрофиле)**](wlan-profileschema-ihv-wlanprofile-element.md)
</dt> </dl>

 

 




