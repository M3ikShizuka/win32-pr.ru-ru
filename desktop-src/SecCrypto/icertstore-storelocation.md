---
description: Задает или получает расположение CAPICOM \_ \_ -хранилища для хранилища сертификатов.
ms.assetid: 2bb76f51-f092-4dbe-93e9-1fdc185c7c50
title: 'Свойство Ицертсторе:: StoreLocation'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ICertStore.StoreLocation
- ICertStore.get_StoreLocation
- ICertStore.put_StoreLocation
- CertStore.StoreLocation
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 97bca7ed9dae20c129d202910b40f7c26d54a576
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127271019"
---
# <a name="icertstorestorelocation-property"></a>Свойство Ицертсторе:: StoreLocation

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP.\]

Свойство **StoreLocation** задает или получает [**Расположение CAPICOM- \_ хранилища \_**](capicom-store-location.md) для хранилища сертификатов.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
CertStore.StoreLocation As CAPICOM_STORE_LOCATION
```



## <a name="property-value"></a>Значение свойства

Расположение хранилища сертификатов.

## <a name="error-codes"></a>Коды ошибок

Если методы доступа к свойству **помещают \_ StoreLocation** и **Get \_ StoreLocation** , они возвращают S \_ ОК.

Любое другое значение **HRESULT** указывает на сбой вызова.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|----------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ицертсторе**](icertstore.md)
</dt> </dl>

 

 




