---
description: В следующем примере функция Верифиверсионинфо используется для определения того, установлены ли указанные наборы продуктов на локальном компьютере.
ms.assetid: 9f405e99-28f5-4415-a274-682b87ae6842
title: Обнаружение набора продуктов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 594acbe22283e1c2a3be3ce60116076b2de6f3fd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056844"
---
# <a name="detecting-a-product-suite"></a>Обнаружение набора продуктов

В следующем примере функция [**верифиверсионинфо**](/windows/desktop/api/Winbase/nf-winbase-verifyversioninfoa) используется для определения того, установлены ли указанные наборы продуктов на локальном компьютере.

В этом примере используется \_ флаг ver и. Если в маске набора указаны два флага, функция возвращает **значение true** только в случае наличия обоих наборов продуктов. Если этот пример был изменен для использования версии \_ или флага, [**Верифиверсионинфо**](/windows/desktop/api/Winbase/nf-winbase-verifyversioninfoa) возвратит **значение true** , если имеется один из наборов продуктов.


```C++
#include <windows.h>
#include <stdio.h>

BOOL CheckProductSuite ( WORD wSuite ) 
{
  OSVERSIONINFOEX osvi;
  DWORDLONG dwlConditionMask = 0;

  // Initialize the OSVERSIONINFOEX structure.

  ZeroMemory(&osvi, sizeof(OSVERSIONINFOEX));
  osvi.dwOSVersionInfoSize = sizeof(OSVERSIONINFOEX);
  osvi.wSuiteMask = wSuite;

  // Set up the condition mask.

  VER_SET_CONDITION( dwlConditionMask, 
          VER_SUITENAME, VER_AND );

  // Perform the test.

  return VerifyVersionInfo(
          &osvi, 
          VER_SUITENAME,
          dwlConditionMask);
}

void main()
{
    if( CheckProductSuite(VER_SUITE_ENTERPRISE) )
        printf( "The system meets the requirements.\n" );
    else printf( "The system does not meet the requirements.\n");
}
```



 

 



