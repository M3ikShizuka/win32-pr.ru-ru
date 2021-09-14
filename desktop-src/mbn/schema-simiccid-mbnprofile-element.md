---
description: Определяет идентификационный номер SIM-карты для устройств GSM.
ms.assetid: 980afba4-fc31-4da0-ba01-6eb8e3db0ac8
title: СимикЦид (Мбнпрофиле), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SimIccID
api_type:
- Schema
ms.openlocfilehash: f566253ad3e86b4f7ee7317cf125d9e649034847
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252529"
---
# <a name="simiccid-mbnprofile-element"></a>СимикЦид (Мбнпрофиле), элемент

Элемент **симикЦид (мбнпрофиле)** определяет идентификационный номер SIM-карты для устройств GSM.

Этот элемент является необязательным и задается службой мобильного широкополосного подключения для внутреннего использования. Приложение не должно задавать это поле при создании или обновлении профиля.

``` syntax
<xs:element name="SimIccID"
    type="simIccIDType"
 />
```

Элемент **симикЦид** определяется элементом [**мбнпрофиле**](schema-mbnprofile-element.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**мбнпрофиле**](schema-mbnprofile-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**мбнпрофиле**](schema-mbnprofile-element.md)
</dt> </dl>

 

 




