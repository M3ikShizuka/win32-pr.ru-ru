---
title: ремотесервернаме
description: Настраивает Клиент для запроса запуска объекта на определенном компьютере при вызове функции активации, для которой не указана структура КОСЕРВЕРИНФО.
ms.assetid: 0413564e-e8ba-4e6e-ad29-62997c63aab3
keywords:
- COM-значение реестра Ремотесервернаме
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0634d858b04fbbdf5d3a6024dbd9fdea4ee06d99
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053144"
---
# <a name="remoteservername"></a>ремотесервернаме

Настраивает Клиент для запроса запуска объекта на определенном компьютере при вызове функции активации, для которой не указана структура [**косерверинфо**](/windows/win32/api/objidlbase/ns-objidlbase-coserverinfo) .

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\AppID
   {AppID_GUID}
      RemoteServerName = name
```

## <a name="remarks"></a>Комментарии

**Ремотесервернаме** обеспечивает простое управление конфигурацией клиентских приложений; они могут быть написаны без жестко заданных имен серверов и могут быть настроены путем изменения значений реестра **ремотесервернаме** классов объектов, которые они используют.

Как описано в документации по перечислению [**клскткс**](/windows/win32/api/wtypesbase/ne-wtypesbase-clsctx) и структуре [**косерверинфо**](/windows/win32/api/objidlbase/ns-objidlbase-coserverinfo) , один из параметров распределенной активации com является указателем на структуру **косерверинфо** . Если это значение не **равно NULL**, информация в структуре **косерверинфо** переопределяет значение ключа **ремотесервернаме** для вызова функции.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Регистрация серверов COM](registering-com-servers.md)
</dt> </dl>

 

 