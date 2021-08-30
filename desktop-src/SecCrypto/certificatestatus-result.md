---
description: Свойство Result получает значение, указывающее, действителен ли сертификат. Это свойство по умолчанию.
ms.assetid: b1edfbde-9d54-4e9c-ba9b-33e4c354c23f
title: Цертификатестатус. Result, свойство
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CertificateStatus.Result
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: dd67cd554fce84edc61b1b48e8a539b58a330ec1163b87b17dd8847b31fb15e8
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119993224"
---
# <a name="certificatestatusresult-property"></a>Цертификатестатус. Result, свойство

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP. Вместо этого используйте [**структуру X509ChainStatus**](/dotnet/api/system.security.cryptography.x509certificates.x509chainstatus?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Свойство **result** получает значение, указывающее, действителен ли сертификат. Это свойство по умолчанию.

## <a name="syntax"></a>Синтаксис


```VB
CertificateStatus.Result As Boolean
```



## <a name="property-value"></a>Значение свойства

**Значение true** показывает, что сертификат действителен. Срок действия сертификата проверяется с использованием текущего значения свойства [**чеккфлаг**](certificatestatus-checkflag.md) и различных параметров политики.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------------------|----------------------------------------------------------------------------------------|
| Окончание поддержки клиента<br/> | Windows Vista<br/>                                                               |
| Поддержка конца сервера<br/> | Windows Server 2008<br/>                                                         |
| Распространяемые компоненты<br/>       | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



 

 
