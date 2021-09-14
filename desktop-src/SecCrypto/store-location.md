---
description: Извлекает расположение хранилища сертификатов, которое представляет этот объект.
ms.assetid: 756ee7cb-5f9f-4fb2-bf10-79b543895189
title: Свойство Store. Location
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Store.Location
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 42afe40dffde5a0375928d355508ec75a4076f17
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064606"
---
# <a name="storelocation-property"></a>Свойство Store. Location

\[Свойство **Location** доступно для использования в операционных системах, указанных в разделе требования. Вместо этого используйте [**класс X509Store**](/dotnet/api/system.security.cryptography.x509certificates.x509store?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Свойство **Location** извлекает расположение хранилища сертификатов, которое представляет этот объект.

## <a name="syntax"></a>Синтаксис


```VB
Store.Location As CAPICOM_STORE_LOCATION
```



## <a name="property-value"></a>Значение свойства

Значение [**\_ \_ расположения CAPICOM Store**](capicom-store-location.md) , представляющее расположение хранилища сертификатов.

## <a name="remarks"></a>Remarks

Значение свойства **Location** совпадает со значением, заданным для параметра *StoreLocation* метода [**Open**](store-open.md) при открытии хранилища.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|----------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,1 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Хранение**](store.md)
</dt> </dl>

 

 
