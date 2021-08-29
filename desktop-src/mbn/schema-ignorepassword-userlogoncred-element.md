---
description: Указывает способ управления паролями при обновлении профилей.
ms.assetid: 74d7ceb1-d778-4a12-907b-0528d9ff45be
title: Игнорепассворд (Усерлогонкред), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IgnorePassword
api_type:
- Schema
ms.openlocfilehash: 683fafb763e3f8613afa1b8dca99020856d67a03fdb44e993adf032ce166ceab
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118975173"
---
# <a name="ignorepassword-userlogoncred-element"></a>Игнорепассворд (Усерлогонкред), элемент

Элемент **игнорепассворд (усерлогонкред)** определяет способ управления паролями при обновлении профилей.

Если задано значение **true** и профиль с тем же именем существует во время операции обновления, то пароль из этого профиля будет создан и сохранен в новом профиле.

Этот элемент является необязательным.

``` syntax
<xs:element name="IgnorePassword"
    type="boolean"
 />
```

Элемент **игнорепассворд** определяется элементом [**усерлогонкред**](schema-userlogoncred-contexttype-element.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                         |



## <a name="see-also"></a>См. также

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**UserLogonCred**](schema-userlogoncred-contexttype-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Усерлогонкред (contextType)**](schema-userlogoncred-contexttype-element.md)
</dt> </dl>

 

 




