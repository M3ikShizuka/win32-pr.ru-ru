---
title: Синхронизация обратного вызова
description: Синхронизация обратного вызова
ms.assetid: e8268f18-49e7-4e09-9006-77858b734bf4
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4f85f388a81b6568db502b4f9843cc7fb9135bfaa9f3529a301993aeac87c43c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119859644"
---
# <a name="callback-synchronization"></a>Синхронизация обратного вызова

Асинхронный [API-интерфейс WinInet](/windows/desktop/WinInet/portal) (используемый для наиболее распространенных протоколов) оставляет синхронизацию механизма обратного вызова и вызывающего приложения в качестве упражнения для клиента. Это сделано намеренно, так как оно обеспечивает максимальную степень гибкости. Протоколы по умолчанию и реализация моникера URL выполняют эту синхронизацию и гарантируют, что приложения с одним потоком и потоковыми потоками никогда не должны справляться с состязаниями в стиле свободной цепочки. То есть интерфейсы [**иенумформатетк**](/windows/desktop/api/ObjIdl/nn-objidl-ienumformatetc) и [**метода интерфейса IBindStatusCallback**](/previous-versions/windows/internet-explorer/ie-developer/platform-apis/ms775060(v=vs.85)) клиента вызываются только в соответствующих потоках. Эта функция прозрачна для пользователя URL-адреса Ммоникер, если каждый поток, вызывающий [**IMoniker:: биндтостораже**](/windows/desktop/api/ObjIdl/nf-objidl-imoniker-bindtostorage) и [**IMoniker:: биндтубжект**](/windows/desktop/api/ObjIdl/nf-objidl-imoniker-bindtoobject) , имеет очередь сообщений.

Для асинхронной спецификации моникера требуется более точный контроль определения приоритетов и управления загрузкой, чем разрешено для WinSock или WinInet. Соответственно, моникер URL-адреса управляет всеми загружаемыми файлами для любого потока вызывающего объекта, используя (в рамках синхронизации) схему приоритета на основе спецификации [**ибиндинг**](/previous-versions/windows/internet-explorer/ie-developer/platform-apis/ms775071(v=vs.85)) .

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Моникеры URL-адресов](url-monikers.md)
</dt> </dl>

 

 