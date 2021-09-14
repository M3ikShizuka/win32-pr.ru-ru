---
description: Содержит имя профиля беспроводной локальной сети.
ms.assetid: b8977183-7b5d-4c79-9065-ade85ed45716
title: Элемент Name (Вланпрофиле)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- name
api_type:
- Schema
api_location: ''
ms.openlocfilehash: 79174d1cb24fff1841b3022fa06e201794415ce5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127245452"
---
# <a name="name-wlanprofile-element"></a>Элемент Name (Вланпрофиле)

Элемент Name (Вланпрофиле) содержит имя профиля беспроводной локальной сети.

``` syntax
<xs:element name="name"
    type="nameType"
 />
```

Элемент **Name** определяется элементом [**вланпрофиле**](wlan-profileschema-wlanprofile-element.md) .

## <a name="remarks"></a>Remarks

В именах учитывается регистр.

для Windows XP с пакетом обновления 3 (sp3) и API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2) элемент name игнорируется при сохранении профиля в хранилище профилей. Имя профиля является производным от SSID сети. Для сетевых профилей инфраструктуры имя профиля — это идентификатор SSID сети. Для сетевых профилей ad hoc имя профиля — это идентификатор SSID нерегламентированной сети, за которым следует `-adhoc` . Escape-символы XML, такие как &, не отображаются. избегайте использования escape-символов XML в именах SSID для профилей, развернутых в Windows XP с SP3 или API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2).

для любого сетевого профиля, предназначенного для использования только в Windows Vista или Windows Server 2008, имя может быть любой строкой.

## <a name="examples"></a>Примеры

Чтобы просмотреть образцы профилей, в которых используется элемент **Name** , см. раздел [образцы профилей беспроводной связи](wireless-profile-samples.md).

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

 

 




