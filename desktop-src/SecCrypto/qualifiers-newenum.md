---
description: '\_Свойство NewEnum квалификаторов Извлекает интерфейс IEnumVARIANT для объекта, который можно использовать для перечисления коллекции. это свойство скрыто в Visual Basic scripting Edition (VBScript).'
ms.assetid: e51f8ca1-ef1f-475b-8368-e8296fae0f04
title: Qualifiers._NewEnum, свойство
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Qualifiers._NewEnum
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 01a4d62604dabacd2d78d5d2f6cbee0db7189196
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173128"
---
# <a name="qualifiers_newenum-property"></a>Квалификаторы. \_ Свойство NewEnum

\[Свойство **\_ NewEnum** доступно для использования в операционных системах, указанных в разделе требования. Вместо этого используйте [**класс X509Extension**](/dotnet/api/system.security.cryptography.x509certificates.x509extension?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) , вызвав конструктор, принимающий OID в качестве параметра, а затем использовать OID для политик сертификатов для обработки квалификаторов, которые являются частью сведений о политике в расширении политик сертификатов.\]

Свойство **\_ NewEnum** Извлекает интерфейс [**IEnumVARIANT**](/windows/win32/api/oaidl/nn-oaidl-ienumvariant) для объекта, который можно использовать для перечисления коллекции. это свойство скрыто в Visual Basic scripting Edition (VBScript).

## <a name="syntax"></a>Синтаксис


```VB
Qualifiers._NewEnum As IUnknown
```



## <a name="property-value"></a>Значение свойства

Интерфейс [**IEnumVARIANT**](/windows/win32/api/oaidl/nn-oaidl-ienumvariant) объекта, который может использоваться для перечисления коллекции.

## <a name="remarks"></a>Remarks

это свойство автоматически используется для внутренних целей при использовании `For Each In` конструкции в Visual Basic scripting Edition (VBScript).

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|----------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Квалификаторы**](qualifiers.md)
</dt> </dl>

 

 
