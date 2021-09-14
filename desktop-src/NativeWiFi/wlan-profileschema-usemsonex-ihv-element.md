---
description: Указывает источник параметров безопасности 802.1 X, используемых компонентом безопасности независимого поставщика оборудования.
ms.assetid: 9c216319-d962-4c68-89a3-116eff3f4376
title: Усемсонекс (IHV), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- useMSOneX
api_type:
- Schema
api_location: ''
ms.openlocfilehash: aa9f2092ac0e76feae89b02f333ae3098288ccef
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067639"
---
# <a name="usemsonex-ihv-element"></a>Усемсонекс (IHV), элемент

Элемент **усемсонекс** (IHV) указывает происхождение параметров безопасности 802.1 x, используемых компонентом безопасности IHV.

Если **усемсонекс** имеет значение true, компоненты безопасности IHV используют определенные корпорацией Майкрософт параметры 802.1 x. Если **усемсонекс** имеет значение false, компоненты безопасности IHV используют предоставленные поставщиком параметры 802.1 x.

**Windows XP с SP3 и API беспроводной локальной сети для Windows XP с пакетом обновления 2 (SP2):** Этот элемент не поддерживается.

``` syntax
<xs:element name="useMSOneX"
    type="boolean"
    minOccurs="0"
 />
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

 

 




