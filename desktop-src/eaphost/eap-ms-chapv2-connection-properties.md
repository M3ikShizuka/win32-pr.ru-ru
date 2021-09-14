---
title: Свойства подключения MS-CHAPv2 EAP
description: Сведения о свойствах подключения EAP MS-CHAPv2. См. пример, который является экземпляром устаревшей схемы mschapv2connectionpropertiesv1.
ms.assetid: d6a057e0-56f6-4a31-9391-fde631ac2898
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e353c4685e131c2e7301db35de26d927b5882c06
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342255"
---
# <a name="eap-ms-chapv2-connection-properties"></a>Свойства подключения MS-CHAPv2 EAP

Этот образец является экземпляром устаревшей схемы [mschapv2connectionpropertiesv1](mschapv2connectionpropertiesv1schema-schema.md) .

``` syntax
  <?xml version="1.0" ?> 
  <EapHostConfig xmlns="https://www.microsoft.com/provisioning/EapHostConfig" 
    xmlns:eapCommon="https://www.microsoft.com/provisioning/EapCommon" 
    xmlns:baseEap="https://www.microsoft.com/provisioning/BaseEapMethodConfig">
    <EapMethod>
      <eapCommon:Type>26</eapCommon:Type> 
      <eapCommon:AuthorId>0</eapCommon:AuthorId> 
    </EapMethod>
    <Config xmlns:baseEap="https://www.microsoft.com/provisioning/BaseEapConnectionPropertiesV1" 
      xmlns:msPeap="https://www.microsoft.com/provisioning/MsPeapConnectionPropertiesV1" 
      xmlns:msChapV2="https://www.microsoft.com/provisioning/MsChapV2ConnectionPropertiesV1">
      <baseEap:Eap>
        <baseEap:Type>26</baseEap:Type> 
        <msChapV2:EapType>
        <msChapV2:UseWinLogonCredentials>false</msChapV2:UseWinLogonCredentials> 
        </msChapV2:EapType>
      </baseEap:Eap>
    </Config>
  </EapHostConfig>
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Свойства соединения](connection-profiles.md)
</dt> <dt>

[EAPHost и схема прежних версий](eaphost-schemas.md)
</dt> </dl>

 

 




