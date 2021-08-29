---
description: Удаляет объект сертификата из коллекции получателей.
ms.assetid: bb75f6d0-4bab-40dd-9d0c-f0431da9c5f3
title: Метод Recipients. Remove
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Recipients.Remove
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 0da608dcafc8fc0c2341a053679dee0f8d2715c34dcbfb28e84bee02aa658093
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118900764"
---
# <a name="recipientsremove-method"></a>Метод Recipients. Remove

\[Метод **Remove** доступен для использования в операционных системах, указанных в разделе требования. Вместо этого используйте [**класс кмсреЦипиентколлектион**](/dotnet/api/system.security.cryptography.pkcs.cmsrecipientcollection?view=dotnet-plat-ext-3.1&preserve-view=true) в пространстве имен [**System. Security. Cryptography. PKCS**](/dotnet/api/system.security.cryptography.pkcs?view=dotnet-plat-ext-3.1&preserve-view=true) .\]

Метод **Remove** удаляет объект [**сертификата**](certificate.md) из коллекции [**получателей**](recipients.md) .

## <a name="syntax"></a>Синтаксис


```VB
Recipients.Remove( _
  ByVal Index _
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Индекс* \[ окне\]
</dt> <dd>

Индекс объекта [**сертификата**](certificate.md) , который необходимо удалить из коллекции.

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

 

 
