---
description: Схема профиля мобильного широкополосного подключения v3.
ms.assetid: f7a3598f-57dd-4178-896f-31b4d2f65e56
title: Схема профиля мобильного широкополосного подключения v3
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ea42c0c4b6384b85e5373d6537f52cf8c9499e8a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168183"
---
# <a name="mobile-broadband-profile-schema-v3"></a>Схема профиля мобильного широкополосного подключения v3

в пространстве имен доступна схема Windows 8Mobile широкополосного профиля версии v3 `https://www.microsoft.com/networking/WWAN/profile/v3` .

-   [Элементы схемы профиля Mobile широкополосной сети v3](mobile-broadband-profile-schema-v3-elements.md)

``` syntax
<xs:schema targetNamespace="https://www.microsoft.com/networking/WWAN/profile/v3" 
    xmlns="https://www.microsoft.com/networking/WWAN/profile/v3"  
    xmlns:xs="https://www.w3.org/2001/XMLSchema" 
    xmlns:WWAN_profile_v2="https://www.microsoft.com/networking/WWAN/profile/v2"  
    elementFormDefault="qualified"> 

    <xs:import namespace="https://www.microsoft.com/networking/WWAN/profile/v2" schemaLocation="WWAN_profile_v2.xsd"/> 

    <!-- Flag to indicate whether this is an additional PDP context profile, default is "false" --> 
    <xs:element name="IsAdditionalPdpContextProfile" type="xs:boolean"/> 
</xs:schema> 
```

 

 



