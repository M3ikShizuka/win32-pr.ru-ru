---
title: Сдвоенные интерфейсы IAccessible и IDispatch
description: Разработчикам сервера необходимо предоставить интерфейс IDispatch интерфейса (COM) уровня "Стандартный" для доступных объектов.
ms.assetid: 043d6777-6f9a-4e93-aadc-9cbe9a9119c4
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 292252bb8445c5934d8f8dc596e0b4f0d1c0d65415ed45dceace3cccb537ddff
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118115547"
---
# <a name="dual-interfaces-iaccessible-and-idispatch"></a>Сдвоенные интерфейсы: IAccessible и IDispatch

Разработчикам сервера необходимо предоставить интерфейс [**IDispatch**](idispatch-interface.md) интерфейса (com) уровня "Стандартный" для доступных объектов. интерфейс IDispatch позволяет клиентским приложениям, написанным на Microsoft Visual Basic и различным языкам сценариев, использовать методы и свойства, предоставляемые методом [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible). Так как доступный объект предоставляет доступ к объекту непрямо через [IDispatch:: Invoke]( /windows/win32/api/oaidl/nf-oaidl-idispatch-invoke) или напрямую с **IAccessible**, говорят, что у него есть сдвоенный интерфейс.

Когда клиенты C/C++ получают указатель интерфейса IDispatch, клиенты могут вызвать [**QueryInterface**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-queryinterface(q)) , чтобы попробовать преобразовать указатель интерфейса IDispatch в указатель интерфейса [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) . Чтобы вызывать методы **IAccessible** косвенно, клиенты C/C++ вызывают IDispatch:: Invoke. Для повышения производительности вызывайте методы **IAccessible** для непосредственного использования объекта.

Список идентификаторов диспетчеризации (DISPID), которые интерфейс **IDispatch** использует для идентификации методов и свойств [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) , см. [в приложении C: идентификаторы DISPID](appendix-c--iaccessible-dispids.md).

> [!Note]  
> В версии 2,0 и более поздних версиях Microsoft Active Accessibility серверы не обязательно полностью реализуют методы [**IDispatch**](idispatch-interface.md) , но могут просто возвращать E \_ нотимпл после инициализации параметров out, как показано в следующем примере.

 


```C++
HRESULT STDMETHODCALLTYPE AccServer::GetTypeInfoCount(UINT* pctinfo)
{
    *pctinfo = 0;
    return E_NOTIMPL;
};
```



 

 