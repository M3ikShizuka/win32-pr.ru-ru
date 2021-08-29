---
description: Получает логическое значение, указывающее, помечено ли расширение как критическое.
ms.assetid: 71f55d63-a51c-472c-81fc-59212c97bb34
title: Свойство Extension. «Critical»
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Extension.IsCritical
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: f37f3c8549835da95949123aecc3a35b2aa896285bd3ec614228a6b851080468
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119006882"
---
# <a name="extensioniscritical-property"></a>Свойство Extension. «Critical»

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP. Вместо этого используйте [**класс X509Extension**](/dotnet/api/system.security.cryptography.x509certificates.x509extension?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Свойство « **Critical** » получает логическое значение, указывающее, помечено ли расширение как критическое.

## <a name="syntax"></a>Синтаксис


```VB
Extension.IsCritical As Boolean
```



## <a name="property-value"></a>Значение свойства

Если **значение равно true**, расширение помечено как критическое.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------------|----------------------------------------------------------------------------------------|
| Окончание поддержки клиента<br/> | Windows Vista<br/>                                                               |
| Поддержка конца сервера<br/> | Windows Server 2008<br/>                                                         |
| Распространяемые компоненты<br/>       | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



 

 
