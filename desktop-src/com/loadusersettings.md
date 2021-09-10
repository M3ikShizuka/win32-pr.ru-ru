---
title: лоадусерсеттингс
description: Определяет, будет ли COM загружать профиль пользователя для COM-серверов, запущенных в качестве запускающего удостоверения пользовательского приложения.
ms.assetid: 3e2b3249-3747-4d98-96da-f3e480a51d12
keywords:
- COM-значение реестра Лоадусерсеттингс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5e14282b00bc2c2d9b989e19480047f115623d55
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369730"
---
# <a name="loadusersettings"></a>лоадусерсеттингс

Определяет, будет ли COM загружать профиль пользователя для COM-серверов, запущенных в качестве запускающего удостоверения пользовательского приложения.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\AppID
   {AppID_GUID}
      LoadUserSettings = value
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ DWORD** . Если *значение* не равно нулю, com загружает профиль учетной записи пользователя, с помощью которой он запускает COM-сервер. Если *значение* равно нулю или отсутствует, com не будет загружать профиль учетной записи пользователя, с помощью которой он запускает COM-сервер.

Этот параметр игнорируется, если имеется запись [**запуска от имени**](runas.md) .

 

 




