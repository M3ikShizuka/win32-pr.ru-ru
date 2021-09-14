---
description: Возвращает коллекцию EKU для сертификата.
ms.assetid: 64211a00-7d4d-4381-a134-9cd570ed7dbb
title: Екстендедкэйусаже. EKU, свойство
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ExtendedKeyUsage.EKUs
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 24bcf7b4332e75afad0e21415a7dfe8eb690c32b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127253459"
---
# <a name="extendedkeyusageekus-property"></a>Екстендедкэйусаже. EKU, свойство

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP. Вместо этого используйте [**класс X509EnhancedKeyUsageExtension**](/dotnet/api/system.security.cryptography.x509certificates.x509enhancedkeyusageextension?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Свойство **EKU** Возвращает коллекцию [**EKU**](ekus.md) для сертификата.

## <a name="syntax"></a>Синтаксис


```VB
ExtendedKeyUsage.EKUs As EKUs
```



## <a name="property-value"></a>Значение свойства

Коллекция [**EKU**](ekus.md) , содержащая объекты [**EKU**](eku.md) для сертификата.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------------|----------------------------------------------------------------------------------------|
| Окончание поддержки клиента<br/> | Windows Vista<br/>                                                               |
| Поддержка конца сервера<br/> | Windows Server 2008<br/>                                                         |
| Распространяемые компоненты<br/>       | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**екстендедкэйусаже**](extendedkeyusage.md)
</dt> </dl>

 

 
