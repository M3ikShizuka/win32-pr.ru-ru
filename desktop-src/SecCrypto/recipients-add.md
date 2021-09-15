---
description: Добавляет объект сертификата в коллекцию получателей.
ms.assetid: 2a1b9e0f-ccbf-4042-871b-397de6b6fc35
title: Метод Recipients. Add
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Recipients.Add
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 255d17485e3423d50cd86b092c2120605f0f1106
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469850"
---
# <a name="recipientsadd-method"></a>Метод Recipients. Add

\[Метод **Add** доступен для использования в операционных системах, указанных в разделе требования. Вместо этого используйте [**класс кмсреЦипиентколлектион**](/dotnet/api/system.security.cryptography.pkcs.cmsrecipientcollection?view=dotnet-plat-ext-3.1&preserve-view=true) в пространстве имен [**System. Security. Cryptography. PKCS**](/dotnet/api/system.security.cryptography.pkcs?view=dotnet-plat-ext-3.1&preserve-view=true) .\]

Метод **Add** добавляет объект [**сертификата**](certificate.md) в коллекцию [**получателей**](recipients.md) .

## <a name="syntax"></a>Синтаксис


```VB
Recipients.Add( _
  ByVal Certificate _
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Сертификат* \[ окне\]
</dt> <dd>

Выражение, которое разрешается в объект [**сертификата**](certificate.md) для добавления в коллекцию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|----------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Криптографические объекты**](cryptography-objects.md)
</dt> <dt>

[**Recipients**](recipients.md)
</dt> </dl>

 

 
