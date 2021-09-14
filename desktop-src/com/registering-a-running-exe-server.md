---
title: Регистрация работающего сервера EXE
description: Регистрация работающего сервера EXE
ms.assetid: 277f44bb-72b7-4409-955d-2cd53bc99467
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: fa0c6cae15818e5cdb3931f71f0d4be1ac1baef6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971320"
---
# <a name="registering-a-running-exe-server"></a>Регистрация работающего сервера EXE

При запуске исполняемого сервера (EXE) он должен вызвать [**CoRegisterClassObject**](/windows/desktop/api/combaseapi/nf-combaseapi-coregisterclassobject), который регистрирует идентификатор CLSID для сервера в том, что называется таблицей класса (другой таблицей, чем у выполняемой таблицы объектов). При регистрации сервера в таблице классов диспетчер управления службами (SCM) может определить, что нет необходимости повторно запускать класс, так как сервер уже запущен. Если сервер не указан в таблице классов, SCM будет проверять реестр на наличие соответствующих значений и запускать сервер, связанный с данным идентификатором CLSID.

Вы передаете [**COREGISTERCLASSOBJECT**](/windows/desktop/api/combaseapi/nf-combaseapi-coregisterclassobject) CLSID для класса и указатель на интерфейс [**IUnknown**](/windows/desktop/api/Unknwn/nn-unknwn-iunknown) . Клиенты, которые впоследствии вызывают [**кожетклассобжект**](/windows/desktop/api/combaseapi/nf-combaseapi-cogetclassobject) с этим идентификатором CLSID, будут получать указатель на запрашиваемый интерфейс, пока безопасность не запрещает ее. (Дополнительные сведения о нескольких функциях создания и активации экземпляров см. в разделе [вспомогательные функции создания экземпляра](instance-creation-helper-functions.md) .)

Сервер для объекта класса должен вызвать [**CoRevokeClassObject**](/windows/desktop/api/combaseapi/nf-combaseapi-corevokeclassobject) , чтобы отозвать объект класса (удалить его регистрацию), если выполняются все приведенные ниже условия.

-   Нет существующих экземпляров определения объекта.
-   Нет блокировок для объекта класса.
-   Приложение, предоставляющее службы объекту класса, не находится под контролем пользователя (не отображается пользователю на экране).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Установка в качестве приложения службы](installing-as-a-service-application.md)
</dt> <dt>

[Регистрация класса при установке](registering-a-class-at-installation.md)
</dt> <dt>

[Регистрация объектов в таблице ROT](registering-objects-in-the-rot.md)
</dt> <dt>

[Самостоятельная регистрация](self-registration.md)
</dt> </dl>

 

 




