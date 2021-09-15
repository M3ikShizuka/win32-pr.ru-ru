---
title: Классификация прокси-серверов и заглушек DCOM
description: Классификация прокси-серверов и заглушек DCOM
ms.assetid: f5d117d6-6c2c-4beb-8869-1581a5b1846f
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 31685cd1318856b9e305246cfebc2cebb3a7874e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459226"
---
# <a name="categorizing-dcom-proxies-and-stubs"></a>Классификация прокси-серверов и заглушек DCOM

DCOM маршалирует ссылки на объекты путем построения объектов OBJREF, содержащих идентификаторы CLSID. Эти идентификаторы CLSID уязвимы для атак безопасности, так как в процессе маршалирования можно загрузить произвольные библиотеки DLL. Однако \_ \_ \_ при вызове [**CoInitializeSecurity**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializesecurity) не может быть задан флаг еоак без пользовательского маршалирования (см. раздел [**\_ \_ возможности проверки подлинности Еоле**](/windows/win32/api/objidlbase/ne-objidlbase-eole_authentication_capabilities)). Установка этого флага помогает защищать серверную безопасность при использовании DCOM, поскольку снижает вероятность выполнения произвольных библиотек DLL. Если этот флаг установлен, сервер разрешает маршалирование только идентификаторов CLSID, реализованных в ole32.dll, comadmin.dll, comsvcs.dll или es.dll или реализующих \_ идентификатор категории МАРШАЛЕРОМ CATID.

\_МАРШАЛЕРУ CATID — это идентификатор GUID категории компонента, который может быть связан с настраиваемым МАРШАЛЕРОМ CLSID. Интерфейсы, настраиваемые с помощью этого идентификатора CLSID, разрешены, если \_ не задано значение еоак без \_ пользовательского \_ маршалирования через [**CoInitializeSecurity**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializesecurity).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Категории компонентов](component-categories.md)
</dt> </dl>

 

 