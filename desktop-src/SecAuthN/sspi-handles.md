---
description: Содержит список дескрипторов, используемых API-интерфейсом SSPI.
ms.assetid: 94b622d0-7c04-4513-841f-0df9b5d49136
title: Дескрипторы SSPI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1e388633cfee0d0f0470e519bac124a0bd1c70fa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146617"
---
# <a name="sspi-handles"></a>Дескрипторы SSPI

SSPI использует следующие типы дескрипторов и указатель на эти дескрипторы:

-   **Сечандле** и **псечандле**
-   **Кредхандле** и **пкредхандле**
-   **Кткссандле** и **пкткссандле**

Эти типы обработчиков и указатели на эти типы обработчиков определяются следующим образом.


```C++
typedef struct _SecHandle {
  ULONG_PTR       dwLower;
  ULONG_PTR       dwUpper;
} SecHandle, * PSecHandle;

typedef SecHandle    CredHandle;
typedef PSecHandle   PCredHandle;

typedef SecHandle    CtxtHandle;
typedef PSecHandle   PCtxtHandle;
```



 

 



