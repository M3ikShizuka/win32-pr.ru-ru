---
title: Свойства пользователя пакета SDK
description: Сведения о свойствах пользователя пакета SDK. См. пример, который является экземпляром собственной схемы еафостусеркредентиалс.
ms.assetid: e8a9656d-48e7-4580-a84d-2b829e7a692f
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b0c8dab154e1ef6c736849720856a23fdfe2e7b3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127341950"
---
# <a name="sdk-user-properties"></a>Свойства пользователя пакета SDK

Этот образец является экземпляром собственной схемы [еафостусеркредентиалс](eaphostusercredentialsschema-schema.md) .

``` syntax
  <?xml version="1.0" ?>  
  <EapHostUserCredentials xmlns="https://www.microsoft.com/provisioning/EapHostUserCredentials" 
    xmlns:eapCommon="https://www.microsoft.com/provisioning/EapCommon" 
    xmlns:baseEap="https://www.microsoft.com/provisioning/BaseEapMethodUserCredentials">
    <EapMethod>
      <eapCommon:Type>40</eapCommon:Type> 
      <eapCommon:AuthorId>100</eapCommon:AuthorId> 
    </EapMethod> 
    <Credentials>
      <EapType>40</EapType> 
      <Identity>test</Identity> 
      <Password>test</Password> 
    </Credentials>
  </EapHostUserCredentials>
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Свойства пользователя](user-profiles.md)
</dt> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> </dl>

 

 




