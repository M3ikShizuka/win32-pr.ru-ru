---
title: сервицепараметерс
description: Указывает параметры командной строки, передаваемые в объект, установленный для использования COM через значение реестра LocalService.
ms.assetid: da11e422-c0f2-4e44-9728-740ea6b61421
keywords:
- COM-значение реестра Сервицепараметерс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 235de1052df72e88e2093647928ed68ab67451cd
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369474"
---
# <a name="serviceparameters"></a>сервицепараметерс

Указывает параметры командной строки, передаваемые в объект, установленный для использования COM через значение реестра [**LocalService**](localservice.md) .

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\AppID
   {AppID_GUID}
      ServiceParameters = parameter
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ SZ** . Эта строка передается в службу в виде аргумента командной строки при запуске.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**локальная служба.**](localservice.md)
</dt> <dt>

[Регистрация серверов COM](registering-com-servers.md)
</dt> </dl>

 

 




