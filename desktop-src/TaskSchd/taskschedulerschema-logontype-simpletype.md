---
title: Простой тип logonType
description: Определяет возможные значения элемента LogonType.
ms.assetid: a08cd549-f45c-4278-a428-1ffe91b67564
keywords:
- планировщик задач простого типа logonType
topic_type:
- apiref
api_name:
- logonType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 58d8c859502e81b5c5101adac3c8c26539870dd5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259176"
---
# <a name="logontype-simple-type"></a>Простой тип logonType

Определяет возможные значения элемента [**LogonType**](taskschedulerschema-logontype-principaltype-element.md) .

``` syntax
<xs:simpleType name="logonType">
    <xs:restriction
        base="string"
    >
        <xs:enumeration
            value="S4U"
         />
        <xs:enumeration
            value="Password"
         />
        <xs:enumeration
            value="InteractiveToken"
         />
        <xs:enumeration
            value="InteractiveTokenOrPassword"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="enumeration-values"></a>Значения перечисления

Простой тип **logonType** определяет следующие значения.



| Значение                      | Описание                                                                                                                                                                                                                                                                                                                                                |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| S4U                        | Пользователь должен войти в систему, используя службу для входа пользователя (S4U). При использовании имени входа S4U система не хранит пароль и не имеет доступа к сети или зашифрованным файлам.<br/>                                                                                                                                                          |
| Пароль                   | Пользователь должен войти в систему, используя пароль.<br/>                                                                                                                                                                                                                                                                                                              |
| интерактиветокен           | Пользователь уже должен войти в систему. Задача будет запущена только в существующем интерактивном сеансе.<br/>                                                                                                                                                                                                                                                   |
| интерактиветокенорпассворд | Больше не используется; в настоящее время совпадает с паролем.<br/> **Windows 10, версия 1511, Windows 10, версия 1507, Windows 8.1, Windows Server 2012 R2, Windows 8, Windows Server 2012, Windows Vista и Windows Server 2008:** Задача будет запущена в существующем интерактивном сеансе или пользователь должен войти в систему с помощью пароля.<br/> <br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Простые типы схемы планировщик задач](task-scheduler-schema-complex-types.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





