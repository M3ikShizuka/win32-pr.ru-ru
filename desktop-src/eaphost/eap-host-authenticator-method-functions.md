---
title: функции метода Authenticator EAPHost
description: дополнительные сведения о функциях API метода EAPHost Authenticator, таких как еапмесодаусентикаторфриеррормемори.
ms.assetid: 319516ee-b21d-4375-8c90-e3abe0a457e8
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 93fac5114085fe6c620084d564bbff97cc3b4535
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571882"
---
# <a name="eaphost-authenticator-method-functions"></a>функции метода Authenticator EAPHost

ниже приведены функции API метода EAPHost Authenticator.



| Функция                                                                                               | Описание                                                                                                                                                                                 |
|--------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**еапмесодаусентикаторбегинсессион**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorbeginsession)                       | Создает новый сеанс проверки подлинности EAP на сервере EAPHost.                                                                                                                             |
| [**еапмесодаусентикаторендсессион**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorendsession)                           | Закрывает сеанс проверки подлинности EAP на сервере EAPHost.                                                                                                                                 |
| [**еапмесодаусентикаторфриеррормемори**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorfreeerrormemory)                 | Выводит выделенную для ошибки память, выданную методом EAP Authenticator.                                                                                                                   |
| [**еапмесодаусентикаторжетаттрибутес**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorgetattributes)                     | Получает массив атрибутов проверки подлинности EAP из метода проверки подлинности EAP.                                                                                                        |
| [**еапмесодаусентикаторжетинфо**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorgetinfo)                                 | Получает набор указателей на функцию для реализации загруженного метода проверки подлинности EAP.                                                                                            |
| [**еапмесодаусентикаторжетресулт**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorgetresult)                             | Получает результат проверки подлинности из метода проверки подлинности EAP.                                                                                                                        |
| [**еапмесодаусентикаторинитиализе**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorinitialize)                           | Инициализирует метод проверки подлинности EAP для сервера EAPHost.                                                                                                                             |
| [**еапмесодаусентикаторинвокеконфигуи**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorinvokeconfigui)                   | Определяет функцию, которая вызывает диалоговое окно пользовательского интерфейса настройки соединения метода EAP на клиенте.                                                                           |
| [**еапмесодаусентикаторрецеивепаккет**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorreceivepacket)                     | Обрабатывает пакет проверки подлинности EAP, полученный сервером EAPHost, и возвращает ответное действие.                                                                                        |
| [**еапмесодаусентикаторсендпаккет**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorsendpacket)                           | Получает пакет проверки подлинности от метода проверки подлинности EAP для отправки на вызывающий объект.                                                                                               |
| [**еапмесодаусентикаторсетаттрибутес**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorsetattributes)                     | Предоставляет обновленные атрибуты проверки подлинности EAP для установки в методе EAP Authenticator.                                                                                                      |
| [**еапмесодаусентикаторшутдовн**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorshutdown)                               | Завершает работу метода проверки подлинности EAP и готовится к выгрузке с сервера EAPHost.                                                                                                  |
| [**еапмесодаусентикаторупдатеиннермесодпарамс**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorupdateinnermethodparams) | Обновляет параметры сеанса проверки подлинности EAP, ранее установленные с помощью вызова [**еапмесодаусентикаторбегинсессион**](/previous-versions/windows/desktop/api/eapmethodauthenticatorapis/nf-eapmethodauthenticatorapis-eapmethodauthenticatorbeginsession) на сервере EAPHost. |



 

 

 




