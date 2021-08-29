---
title: Сложный тип Тлсекстенсионстипе
description: Сведения о сложном типе Тлсекстенсионстипе. Этот тип обеспечивает будущие улучшения схемы.
ms.assetid: 5e4f8ef8-1adb-4683-8001-ba7d2d392523
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f9ac12ad6d3b1229f4fcb75506a9e7ae7655db0287ad58fa9a8079ba12c14e99
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118984107"
---
# <a name="tlsextensionstype-complex-type"></a>Сложный тип Тлсекстенсионстипе

Сложный тип **тлсекстенсионстипе** обеспечивает будущие улучшения схемы.


```XML
<xs:complexType name="TLSExtensionsType">
    <xs:sequence>
        <xs:any processContents="lax" 
            minOccurs="0" 
            maxOccurs="unbounded" 
            namespace="##other"
        />
    <xs:sequence>
</xs:complexType>

```



## <a name="remarks"></a>Remarks

Элемент **тлсекстенсионстипе** является необязательным.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>


</dt> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> <dt>

[eaptlsconnectionpropertiesv2](eaptlsconnectionpropertiesv2schema-schema.md)
</dt> <dt>

[Сложные типы eaptlsconnectionpropertiesv2](eaptlsconnectionpropertiesv2schema-complex-types.md)
</dt> <dt>

[**Тлсекстенсионс (Тлсекстенсионстипе)**](eaptlsconnectionpropertiesv2schema-performservervalidation-eaptype-element.md)
</dt> </dl>

 

 




