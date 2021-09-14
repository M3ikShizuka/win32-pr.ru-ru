---
title: Password (Еаптипе), элемент
description: Сведения об элементе Password (Еаптипе). Этот элемент определяет пароль пользователя или компьютера, для которого выполняется проверка подлинности.
ms.assetid: d3ad95b8-2d98-420f-a680-a83b49ae2992
keywords:
- Элемент Password EAPHost
topic_type:
- apiref
api_name:
- Password
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 6da29146be7ed2f0c17d7311f79921b44cd0929e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126963413"
---
# <a name="password-eaptype-element"></a>Password (Еаптипе), элемент

Элемент **Password (еаптипе)** определяет пароль пользователя или компьютера, для которого выполняется проверка подлинности.

``` syntax
<xs:element name="Password"
    type="string"
 />
```

Элемент **Password** определяется элементом [**еаптипе**](mschapv2userpropertiesv1schema-eaptype-element.md) .

## <a name="remarks"></a>Комментарии

Если элемент **Password (еаптипе)** отсутствует, то хэш пароля будет получен из Winlogon. Этот элемент является необязательным.

## <a name="requirements"></a>Требования



| Роль | Минимальная поддерживаемая версия ОС |
|------|------------------------------|
| Клиент<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Сервер<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**еаптипе**](mschapv2userpropertiesv1schema-eaptype-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**еаптипе**](mschapv2userpropertiesv1schema-eaptype-element.md)
</dt> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[Схема mschapv2userpropertiesv1](mschapv2userpropertiesv1schema-schema.md)
</dt> </dl>

 

 





