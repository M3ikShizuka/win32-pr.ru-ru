---
description: Извлекает квалификатор, основанный на указанном индексе.
ms.assetid: 4d54358d-99de-4a1c-b843-41006f47a279
title: Свойство квалификаторов. Item
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Qualifiers.Item
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 798b1f212aabd5b1ab34a1eefb626be4572b9c1b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173132"
---
# <a name="qualifiersitem-property"></a>Свойство квалификаторов. Item

\[Свойство **Item** доступно для использования в операционных системах, указанных в разделе требования. Вместо этого используйте [**класс X509Extension**](/dotnet/api/system.security.cryptography.x509certificates.x509extension?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) , вызвав конструктор, принимающий OID в качестве параметра, а затем использовать OID для политик сертификатов для обработки квалификаторов, которые являются частью сведений о политике в расширении политик сертификатов.\]

Свойство **Item** получает квалификатор, основанный на указанном индексе. Это свойство по умолчанию.

## <a name="syntax"></a>Синтаксис


```VB
Qualifiers.Item( _
  ByVal Index _
) As Variant
```



## <a name="property-value"></a>Значение свойства

Объект [**квалификатора**](qualifier.md) , представляющий индексированный квалификатор коллекции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|----------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Квалификаторы**](qualifiers.md)
</dt> </dl>

 

 
