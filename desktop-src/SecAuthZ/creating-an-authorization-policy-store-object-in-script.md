---
description: Хранилище политик авторизации содержит сведения о политике безопасности приложения или группы приложений.
ms.assetid: bce85da8-11de-4bc1-b097-d8efdbd28abf
title: Создание объекта хранилища политики авторизации в скрипте
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: feb02c80408210b663524e2aa914852a853e80ea
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146325"
---
# <a name="creating-an-authorization-policy-store-object-in-script"></a>Создание объекта хранилища политики авторизации в скрипте

Хранилище политик авторизации содержит сведения о политике безопасности приложения или группы приложений. Эти сведения включают в себя приложения, операции, задачи, пользователей и группы пользователей, связанных с магазином. При инициализации приложения, использующего Диспетчер авторизации, оно загружает эту информацию из хранилища. Хранилище политик авторизации должно находиться в доверенной системе, так как администраторы этой системы имеют высокий уровень доступа к хранилищу.

Диспетчер авторизации поддерживает хранение политики авторизации либо в службе каталогов Active Directory, либо в XML-файле, как показано в следующих примерах. В API диспетчера авторизации хранилище политик авторизации представлено объектом [**азаусоризатионсторе**](/windows/desktop/api/Azroles/nn-azroles-iazauthorizationstore) . В примерах показано, как создать объект **азаусоризатионсторе** для хранилища Active Directory и XML-хранилища.

-   [Создание хранилища Active Directory](#creating-an-active-directory-store)
-   [создание хранилища SQL Server](#creating-a-sql-server-store)
-   [Создание хранилища XML](#creating-an-xml-store)

## <a name="creating-an-active-directory-store"></a>Создание хранилища Active Directory

чтобы использовать Active Directory для хранения политики авторизации, домен должен находиться в режиме работы домена **Windows Server 2003** . Хранилище политик авторизации не может располагаться в **контексте именования, не являющегося доменом** (также называемого секцией приложения). Рекомендуется размещать хранилище в контейнере **данных программы** в новом подразделении, созданном специально для хранилища политик авторизации. Также рекомендуется, чтобы хранилище размещалось в той же локальной сети, что и серверы приложений, использующие хранилище.

В следующем примере показано, как создать объект [**азаусоризатионсторе**](/windows/desktop/api/Azroles/nn-azroles-iazauthorizationstore) , представляющий хранилище политик авторизации в Active Directory. В этом примере предполагается, что существует Active Directory подразделение с именем Program Data в домене с именем authmanager.com.


```VB
'  Create the store object.
Dim authStore
Set authStore = CreateObject("AzRoles.AzAuthorizationStore")

'  Initialize the store object.
authStore.Initialize 1, _
    "msldap://CN=MyStore, CN=Program Data,DC=authmanager,DC=com"

'  Save the information to the store.
authStore.Submit
```



## <a name="creating-a-sql-server-store"></a>создание хранилища SQL Server

диспетчер авторизации поддерживает создание хранилища политик авторизации на основе Microsoft SQL Server. чтобы создать хранилище данных авторизации на основе SQL Server, используйте URL-адрес, который начинается с префикса **MSSQL://**. URL-адрес должен содержать допустимую строку подключения SQL, имя базы данных и имя хранилища политики авторизации: **MSSQL://**_ConnectionString_ *_/_* _DatabaseName_ *_/_* _полицисторенаме_.

если экземпляр SQL Server не содержит указанную базу данных диспетчера авторизации, диспетчер авторизации создает новую базу данных с таким именем.

> [!Note]  
> подключения к хранилищу SQL Server не шифруются, если только не задано явное шифрование SQL для подключения или не настроено шифрование сетевого трафика, использующего протокол IPsec.

 

в следующем примере показано, как создать объект [**азаусоризатионсторе**](/windows/desktop/api/Azroles/nn-azroles-iazauthorizationstore) , представляющий хранилище политик авторизации в базе данных SQL Server.


```VB
'  Create the store object.
Dim authStore
Set authStore = CreateObject("AzRoles.AzAuthorizationStore")

'  Initialize the store object.
authStore.Initialize 1, _ 
  "MSSQL://Driver={SQL Server};Server={AzServer};/AzDB/MyStore"

'  Save information to the store.
authStore.Submit
```



## <a name="creating-an-xml-store"></a>Создание хранилища XML

Диспетчер авторизации поддерживает создание хранилища политик авторизации в формате XML. Хранилище XML может располагаться на том же компьютере, где выполняется приложение, или его можно сохранить удаленно. Непосредственное изменение XML-файла не поддерживается. Чтобы изменить хранилище политик, используйте оснастку MMC диспетчера авторизации или API диспетчера авторизации.

Диспетчер авторизации не поддерживает делегирование администрирования хранилища политик XML. Сведения о делегировании см. [в разделе Делегирование определения разрешений в скрипте](delegating-the-defining-of-permissions-in-script.md).

В следующем примере показано, как создать объект [**азаусоризатионсторе**](/windows/desktop/api/Azroles/nn-azroles-iazauthorizationstore) , представляющий хранилище политики авторизации в XML-файле.


```VB
'  Create the store object.
Dim authStore
Set authStore = CreateObject("AzRoles.AzAuthorizationStore")

'  Initialize the store object.
authStore.Initialize 1, "msxml://C:\MyStore.xml"

'  Save information to the store.
authStore.Submit
```



 

 



