---
description: Содержит политику беспроводной локальной сети.
ms.assetid: 16ffb682-f88b-4ca1-a902-d2db5e347975
title: Вланполици, элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WLANPolicy
api_type:
- Schema
api_location: ''
ms.openlocfilehash: e9e56e25e51a3c6e798242b390f5d8b7341d7306455f1b15eb9e450830d3c9b0
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119064704"
---
# <a name="wlanpolicy-element"></a>Вланполици, элемент

Элемент **вланполици** содержит политику беспроводной локальной сети. Этот элемент является уникальным корневым элементом для профиля политики беспроводной связи.

Целевое пространство имен для элемента **вланполици** — `https://www.microsoft.com/networking/WLAN/policy/v1` .

``` syntax
<xs:element name="WLANPolicy">
    <xs:complexType>
        <xs:sequence>
            <xs:element name="name"
                type="nameType"
             />
            <xs:element name="description"
                type="nameType"
                minOccurs="0"
             />
            <xs:element name="globalFlags">
                <xs:complexType>
                    <xs:sequence>
                        <xs:element name="enableAutoConfig"
                            type="boolean"
                         />
                        <xs:element name="showDeniedNetwork"
                            type="boolean"
                         />
                        <xs:element name="allowEveryoneToCreateAllUserProfiles"
                            type="boolean"
                         />
                        <xs:any
                            processContents="lax"
                            minOccurs="0"
                            maxOccurs="unbounded"
                            namespace="##other"
                         />
                    </xs:sequence>
                </xs:complexType>
            </xs:element>
            <xs:element name="networkFilter"
                minOccurs="0"
            >
                <xs:complexType>
                    <xs:sequence>
                        <xs:element name="allowList"
                            minOccurs="0"
                        >
                            <xs:complexType>
                                <xs:sequence>
                                    <xs:element name="network"
                                        type="networkItemType"
                                        maxOccurs="unbounded"
                                     />
                                    <xs:any
                                        processContents="lax"
                                        minOccurs="0"
                                        maxOccurs="unbounded"
                                        namespace="##other"
                                     />
                                </xs:sequence>
                            </xs:complexType>
                        </xs:element>
                        <xs:element name="blockList"
                            minOccurs="0"
                        >
                            <xs:complexType>
                                <xs:sequence>
                                    <xs:element name="network"
                                        type="networkItemType"
                                        maxOccurs="unbounded"
                                     />
                                    <xs:any
                                        processContents="lax"
                                        minOccurs="0"
                                        maxOccurs="unbounded"
                                        namespace="##other"
                                     />
                                </xs:sequence>
                            </xs:complexType>
                        </xs:element>
                        <xs:element name="denyAllIBSS"
                            type="boolean"
                            minOccurs="0"
                         />
                        <xs:element name="denyAllESS"
                            type="boolean"
                            minOccurs="0"
                         />
                        <xs:any
                            processContents="lax"
                            minOccurs="0"
                            maxOccurs="unbounded"
                            namespace="##other"
                         />
                    </xs:sequence>
                </xs:complexType>
            </xs:element>
            <xs:element name="profileList"
                minOccurs="0"
            >
                <xs:complexType>
                    <xs:sequence>
                        <xs:any
                            processContents="lax"
                            maxOccurs="unbounded"
                            namespace="##other"
                         />
                    </xs:sequence>
                </xs:complexType>
            </xs:element>
            <xs:any
                processContents="lax"
                minOccurs="0"
                maxOccurs="unbounded"
                namespace="##other"
             />
        </xs:sequence>
    </xs:complexType>
</xs:element>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                                                                    | Тип                                                                     | Описание                                                                                                                          |
|----------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| [**алловеверйонетокреатеаллусерпрофилес**](wlan-policyschema-alloweveryonetocreatealluserprofiles-globalflags-element.md) | Логическое                                                                  | Указывает, может ли любой пользователь создать профиль для всех пользователей. <br/>                                                               |
| [**Разрешенных**](wlan-policyschema-allowlist-networkfilter-element.md)                                                     |                                                                          | Список беспроводных ЛОКАЛЬНЫХ сетей, к которым может подключаться любой компьютер. <br/>                                       |
| [**Списка блокировки**](wlan-policyschema-blocklist-networkfilter-element.md)                                                     |                                                                          | Список беспроводных ЛОКАЛЬНЫХ сетей, к которым компьютер не должен подключаться.<br/>                                                    |
| [**деняллесс**](wlan-policyschema-denyalless-networkfilter-element.md)                                                   | Логическое                                                                  | Указывает, заблокирован ли доступ ко всем сетям инфраструктуры. <br/>                                                           |
| [**деняллибсс**](wlan-policyschema-denyallibss-networkfilter-element.md)                                                 | Логическое                                                                  | Указывает, заблокирован ли доступ ко всем компьютерным сетям. <br/>                                                                   |
| [**nописание**](wlan-policyschema-description-wlanpolicy-element.md)                                                    | [**наметипе**](wlan-policyschema-nametype-simpletype.md)                | Описание политики беспроводной локальной сети. <br/>                                                                                |
| [**енаблеаутоконфиг**](wlan-policyschema-enableautoconfig-globalflags-element.md)                                         | Логическое                                                                  | Указывает, используют ли компьютеры встроенную службу автоматической настройки (автоконфигурации) для управления беспроводными подключениями. <br/> |
| [**глобалфлагс**](wlan-policyschema-globalflags-wlanpolicy-element.md)                                                    |                                                                          | Содержит глобальные параметры для модуля автоматической настройки (ACM). <br/>                                                    |
| [**безымян**](wlan-policyschema-name-wlanpolicy-element.md)                                                                  | [**наметипе**](wlan-policyschema-nametype-simpletype.md)                | Имя политики беспроводной локальной сети. <br/>                                                                                       |
| [**сети**](wlan-policyschema-network-allowlist-element.md)                                                             | [**нетворкитемтипе**](wlan-policyschema-networkitemtype-complextype.md) | Разрешенная сеть. <br/>                                                                                                      |
| [**сети**](wlan-policyschema-network-blocklist-element.md)                                                             | [**нетворкитемтипе**](wlan-policyschema-networkitemtype-complextype.md) | Заблокированная сеть. <br/>                                                                                                       |
| [**нетворкфилтер**](wlan-policyschema-networkfilter-wlanpolicy-element.md)                                                |                                                                          | Список разрешенных и запрещенных сетей.<br/>                                                                                  |
| [**профилелист**](wlan-policyschema-profilelist-wlanpolicy-element.md)                                                    |                                                                          | Содержит список профилей, применяемых на уровне домена или компьютера. <br/>                                                |
| [**шовдениеднетворк**](wlan-policyschema-showdeniednetwork-globalflags-element.md)                                       | Логическое                                                                  | указывает, отображаются ли запрещенные сети в мастере **Подключение сети** . <br/>                                         |



## <a name="remarks"></a>Remarks

Сведения о просмотре списка дочерних элементов в древовидной структуре см. в разделе [ \_ элементы схемы политики WLAN](wlan-policyschema-elements.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 




