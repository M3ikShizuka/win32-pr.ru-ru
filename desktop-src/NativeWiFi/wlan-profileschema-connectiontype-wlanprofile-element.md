---
description: Указывает режим работы сети.
ms.assetid: b71de38a-6373-4d96-90dd-a3ad4a7de074
title: Элемент connectionType (Вланпрофиле)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- connectionType
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 1e7b456260c656ebb3d64b6a3732fe97ca3ca488
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127245545"
---
# <a name="connectiontype-wlanprofile-element"></a>Элемент connectionType (Вланпрофиле)

Элемент connectionType (Вланпрофиле) указывает режим работы сети.

Значение **ESS** указывает на сеть инфраструктуры, а **ибсс** — на нерегламентированную сеть.

``` syntax
<xs:element name="connectionType">
    <xs:simpleType>
        <xs:restriction
            base="string"
        >
            <xs:enumeration
                value="IBSS"
             />
            <xs:enumeration
                value="ESS"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент **connectionType** определяется элементом [**вланпрофиле**](wlan-profileschema-wlanprofile-element.md) .

## <a name="examples"></a>Примеры

Чтобы просмотреть образцы профилей, в которых используется элемент **connectionType** , см. раздел [образцы профилей беспроводной связи](wireless-profile-samples.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista, Windows XP с пакетом обновления 3 (SP3), \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                |
| Распространяемые компоненты<br/>          | API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2)<br/>                 |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**WLANProfile**](wlan-profileschema-wlanprofile-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**WLANProfile**](wlan-profileschema-wlanprofile-element.md)
</dt> </dl>

 

 




