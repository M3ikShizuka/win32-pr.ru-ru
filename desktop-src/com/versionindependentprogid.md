---
title: версиониндепендентпрогид
description: Связывает идентификатор ProgID с идентификатором CLSID. Это значение используется для определения последней версии объектного приложения.
ms.assetid: 5d188db9-ea4f-47fe-882f-a6caa7e86a25
keywords:
- COM раздела реестра Версиониндепендентпрогид
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a5774dfa5202521bb5055bab6a62aa7c6a60b3cc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971296"
---
# <a name="versionindependentprogid"></a>версиониндепендентпрогид

Связывает идентификатор ProgID с идентификатором CLSID. Это значение используется для определения последней версии объектного приложения.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      VersionIndependentProgID = Program.Component
```

## <a name="remarks"></a>Комментарии

Это значение **reg \_ SZ** , которое указывает последнюю версию приложения объекта.

Идентификатор ProgID, не зависящий от версии, хранится и обслуживается исключительно кодом приложения. При задании идентификатора ProgID, не зависящего от версии, функция [**клсидфромпрогид**](/windows/desktop/api/combaseapi/nf-combaseapi-clsidfromprogid) возвращает идентификатор CLSID текущей версии.

Для преобразования между этими двумя представлениями можно использовать [**клсидфромпрогид**](/windows/desktop/api/combaseapi/nf-combaseapi-clsidfromprogid) и [**прогидфромклсид**](/windows/desktop/api/combaseapi/nf-combaseapi-progidfromclsid) .

 

 




