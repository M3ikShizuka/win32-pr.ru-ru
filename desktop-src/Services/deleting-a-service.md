---
description: Программа настройки службы использует функцию OpenService для получения маркера установленного объекта службы. Затем программа может использовать в функции DeleteService обработчик объекта службы, чтобы удалить службу из базы данных SCM.
ms.assetid: 3bfe4d42-a8a0-4613-9b0f-a80eef54b622
title: Удаление службы
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 40b1e0e95e0ea943487a0d3fa513afa2c0563d3c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127265059"
---
# <a name="deleting-a-service"></a>Удаление службы

[Программа настройки службы](service-configuration-programs.md) использует функцию [**OpenService**](/windows/desktop/api/Winsvc/nf-winsvc-openservicea) для получения маркера установленного объекта службы. Затем программа может использовать в функции [**DeleteService**](/windows/desktop/api/Winsvc/nf-winsvc-deleteservice) обработчик объекта службы, чтобы удалить службу из базы данных SCM.

Функция Доделетесвк в следующем примере показывает, как удалить службу из базы данных SCM. Переменная Сзсвкнаме представляет собой глобальную переменную, которая содержит имя удаляемой службы. Полный пример, задающий эту переменную, см. в разделе [свкконфиг. cpp](svcconfig-cpp.md).


```C++
//
// Purpose: 
//   Deletes a service from the SCM database
//
// Parameters:
//   None
// 
// Return value:
//   None
//
VOID __stdcall DoDeleteSvc()
{
    SC_HANDLE schSCManager;
    SC_HANDLE schService;
    SERVICE_STATUS ssStatus; 

    // Get a handle to the SCM database. 
 
    schSCManager = OpenSCManager( 
        NULL,                    // local computer
        NULL,                    // ServicesActive database 
        SC_MANAGER_ALL_ACCESS);  // full access rights 
 
    if (NULL == schSCManager) 
    {
        printf("OpenSCManager failed (%d)\n", GetLastError());
        return;
    }

    // Get a handle to the service.

    schService = OpenService( 
        schSCManager,       // SCM database 
        szSvcName,          // name of service 
        DELETE);            // need delete access 
 
    if (schService == NULL)
    { 
        printf("OpenService failed (%d)\n", GetLastError()); 
        CloseServiceHandle(schSCManager);
        return;
    }

    // Delete the service.
 
    if (! DeleteService(schService) ) 
    {
        printf("DeleteService failed (%d)\n", GetLastError()); 
    }
    else printf("Service deleted successfully\n"); 
 
    CloseServiceHandle(schService); 
    CloseServiceHandle(schSCManager);
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Установка, удаление и перечисление служб](service-installation-removal-and-enumeration.md)
</dt> <dt>

[Полный пример службы](the-complete-service-sample.md)
</dt> </dl>

 

 



