---
description: LSA предоставляет функции, которые администраторы могут использовать для запроса и установки глобальных сведений о политике для локального компьютера и домена.
ms.assetid: bbe27d16-0a6b-435a-ae80-5e983047b511
title: Управление сведениями о политике
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8fdc76137f41c592370dbeecafd243f11012cb1e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067067"
---
# <a name="managing-policy-information"></a>Управление сведениями о политике

LSA предоставляет функции, которые администраторы могут использовать для запроса и установки глобальных сведений о политике для локального компьютера и домена.

Прежде чем можно будет управлять сведениями о политике, приложение должно получить обработчик для объекта локальной [**политики**](policy-object.md) , как показано при [открытии обработчика объектов политики](opening-a-policy-object-handle.md). Этот обработчик необходим для функций, управляющих сведениями о политиках.

Чтобы получить сведения о локальной политике безопасности, вызовите [**лсакуеринформатионполици**](/windows/desktop/api/ntsecapi/nf-ntsecapi-lsaqueryinformationpolicy). Чтобы задать локальную политику безопасности, вызовите [**лсасетинформатионполици**](/windows/desktop/api/ntsecapi/nf-ntsecapi-lsasetinformationpolicy). Описание перечисления [**\_ \_ класс сведений о политике**](/windows/desktop/api/Ntsecapi/ne-ntsecapi-policy_information_class) содержит сведения о типах политик, которые можно запрашивать или задавать.

В следующем примере показано, как получить сведения о домене учетной записи системы, используя обработчик для объекта [**политики**](policy-object.md) системы.


```C++
#include <windows.h>

BOOL GetAccountDomainInfo(LSA_HANDLE PolicyHandle)
{
  NTSTATUS ntsResult = STATUS_SUCCESS;
  PPOLICY_ACCOUNT_DOMAIN_INFO pPADInfo = NULL;
  PWCHAR name = NULL;
  UINT nameSize;
  
  ntsResult = LsaQueryInformationPolicy(
    PolicyHandle,                   // Open handle to a Policy object.
    PolicyAccountDomainInformation, // The information to get.
    (PVOID *)&pPADInfo              // Storage for the information.
  );

  if (ntsResult == STATUS_SUCCESS)
  {  
    // There is no guarantee that the LSA_UNICODE_STRING buffer
    // is null-terminated, so copy the name to a buffer that is.
    nameSize =  pPADInfo->DomainName.Length + 1 * sizeof(WCHAR);
    name = (WCHAR *) LocalAlloc(LPTR, nameSize);
    if (!name)
    {
        wprintf(L"Failed LocalAlloc\n");
        exit(1);
    }
    wcsncpy_s(name, nameSize, pPADInfo->DomainName.Buffer,
        pPADInfo->DomainName.Length);
    wprintf(L"The account domain name is %ws\n", name);
    LocalFree(name);
    if (STATUS_SUCCESS != LsaFreeMemory(pPADInfo))
        wprintf(L"LsaFreeMemory error\n");
  }
  else
  {
    // Show the corresponding win32 error code.
    wprintf(
        L"Error obtaining account domain information - (win32) %lu\n",
        LsaNtStatusToWinError(ntsResult));
  }

  return !ntsResult;
}

```



 

 
