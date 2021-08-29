---
title: Реализация IClassFactory
description: Реализация IClassFactory
ms.assetid: 96466756-c135-4ee5-a48c-f31129878473
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 73b3d524bc65657e973771f2893d562f0ce0095cbfd7fb976ce82cce202794a1
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119756274"
---
# <a name="implementing-iclassfactory"></a>Реализация IClassFactory

Когда клиент использует идентификатор CLSID для запроса создания экземпляра объекта, первым шагом является создание объекта класса, промежуточного объекта, который содержит реализацию методов интерфейса [**IClassFactory**](/windows/win32/api/unknwn/nn-unknwn-iclassfactory) . Хотя модель COM предоставляет несколько функций создания экземпляров, первый шаг в реализации этих функций — это создание объекта класса.

В результате все серверы должны реализовывать методы интерфейса [**IClassFactory**](/windows/win32/api/unknwn/nn-unknwn-iclassfactory) , который содержит два метода:

-   [**CreateInstance**](/windows/desktop/api/Unknwn/nf-unknwn-iclassfactory-createinstance). Этот метод должен создать неинициализированный экземпляр объекта и вернуть указатель на запрошенный интерфейс для объекта.
-   [**Локксервер**](/windows/win32/api/unknwn/nf-unknwn-iclassfactory-lockserver). Этот метод просто увеличивает счетчик ссылок на объект класса, чтобы убедиться, что сервер остается в памяти и не завершает работу до того, как клиент будет готов.

Чтобы сервер был ответственным за собственное лицензирование, COM определяет [**IClassFactory2**](/windows/desktop/api/OCIdl/nn-ocidl-iclassfactory2), который наследует определение от [**IClassFactory**](/windows/win32/api/unknwn/nn-unknwn-iclassfactory). Таким же, сервер, реализующий **IClassFactory2** , должен по определению реализовывать методы **IClassFactory**.

COM также предоставляет вспомогательные функции для реализации серверов вне процесса. Дополнительные сведения см. в разделе [вспомогательные методы реализации сервера](out-of-process-server-implementation-helpers.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Обязанности сервера COM](com-server-responsibilities.md)
</dt> <dt>

[Лицензирование и IClassFactory2](licensing-and-iclassfactory2.md)
</dt> </dl>

 

 