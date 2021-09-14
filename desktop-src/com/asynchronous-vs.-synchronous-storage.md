---
title: асинхронные и синхронные служба хранилища
description: асинхронные и синхронные служба хранилища
ms.assetid: de8c50f8-1733-439f-ab53-f98ac21a1fae
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 884b8613bebf8ef401f76e4761f48fa0ddd831c2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346007"
---
# <a name="asynchronous-and-synchronous-storage"></a>асинхронные и синхронные служба хранилища

асинхронные моникеры также могут возвращать [асинхронный объект служба хранилища](/windows/desktop/Stg/asynchronous-storage) в уведомлении [**метода интерфейса ibindstatuscallback:: ондатааваилабле**](/previous-versions/windows/internet-explorer/ie-developer/platform-apis/ms775061(v=vs.85)) . Этот объект хранилища может разрешить доступ к некоторым из постоянных данных объекта, пока привязка еще выполняется. Клиент может выбрать один из двух режимов хранения: Блокировка и неблокировка.

В режиме блокировки, который совместим с текущими реализациями объектов хранилища, если данные недоступны, вызов блокируется до поступления данных. В неблокирующем режиме, вместо того чтобы блокировать вызов, объект хранилища возвращает новую ошибку E Pending, \_ когда данные недоступны. Клиент, осведомленный о асинхронной привязке и хранилище, задерживает эту ошибку и ожидает дальнейших уведомлений ([**ондатааваилабле**](/previous-versions/windows/internet-explorer/ie-developer/platform-apis/ms775061(v=vs.85))), чтобы повторить операцию. Клиент может выбрать между синхронным (блокирующее) и асинхронным (неблочным) хранилищем, выбрав, следует ли установить \_ флаг биндф асинкстораже в значении *грфбиндф* , возвращаемом в [**метода интерфейса IBindStatusCallback:: GetBindInfo**](/previous-versions/windows/internet-explorer/ie-developer/platform-apis/ms775058(v=vs.85)).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Асинхронные моникеры](asynchronous-monikers.md)
</dt> </dl>

 

 