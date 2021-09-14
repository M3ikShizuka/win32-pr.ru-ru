---
description: Возвращает имя хранилища сертификатов, которое представляет этот объект.
ms.assetid: db61b464-0e8e-4b19-be12-04e00d6bba53
title: Store.Name, свойство
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Store.Name
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 85679bb594bdb59c41773b7f956deea95021381f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064601"
---
# <a name="storename-property"></a>Store.Name, свойство

\[Свойство [**Name**](store-location.md) доступно для использования в операционных системах, указанных в разделе требования. Вместо этого используйте [**класс X509Store**](/dotnet/api/system.security.cryptography.x509certificates.x509store?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Свойство [**Name**](store-location.md) извлекает имя хранилища сертификатов, которое представляет этот объект.

## <a name="syntax"></a>Синтаксис


```VB
Store.Name As String
```



## <a name="property-value"></a>Значение свойства

**Строковое** значение, представляющее имя хранилища сертификатов.

## <a name="remarks"></a>Remarks

Примерами имен хранилищ сертификатов являются My и root.

Значение свойства [**Name**](store-location.md) совпадает со значением, заданным для параметра *StoreName* метода [**Open**](store-open.md) при открытии хранилища.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|----------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,1 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Хранение**](store.md)
</dt> </dl>

 

 
