---
description: Перечисление, описывающее тип сетевого подключения, к которому применим профиль.
MS-HAID: WWAN\_profile\_v4.simpleType\_iwlanApplicabilityType
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: Простой тип Ивланаппликабилититипе
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 529ae39c2b0e137825e7a80d41c43203b0a27de7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469314"
---
# <a name="span-idwwan_profile_v4simpletype_iwlanapplicabilitytypespaniwlanapplicabilitytype-simple-type"></a><span id="WWAN_profile_v4.simpleType_iwlanApplicabilityType"></span>Простой тип Ивланаппликабилититипе

Перечисление, описывающее тип сетевого подключения, к которому применим профиль.

``` syntax
<xs:simpleType name="iwlanApplicabilityType">
    <xs:restriction
        base="token"
    >
        <xs:enumeration
            value="CellularOnly"
         />
        <xs:enumeration
            value="CellularAndIwlan"
         />
        <xs:enumeration
            value="IwlanOnly"
         />
    </xs:restriction>
</xs:simpleType>
```

## <a name="enumeration-values"></a>Значения перечисления

Простой тип **ивланаппликабилититипе** определяет следующие значения.


| Значение | Описание | 
|-------|-------------|
| целлуларонли | <p>Профиль действителен только для подключений по сотовой сети.</p> | 
| целлуларандивлан | <p>Профиль действителен для сотовой сети или Wi-Fi разгрузки подключений.</p> | 
| ивланонли | <p>Профиль действителен только для Wi-Fi разгрузок подключений.</p> | 


 

 



