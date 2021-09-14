---
title: Элемент ID (Нетворксеттингстипе)
description: Содержит значение идентификатора GUID, определяющее сетевой профиль.
ms.assetid: 527912ab-9a81-4570-91c5-8f5943e79a28
keywords:
- Элемент ID планировщик задач
topic_type:
- apiref
api_name:
- Id
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3d14865d50e9c3418e3ef65cdbeaea747a98a4ab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259272"
---
# <a name="id-networksettingstype-element"></a>Элемент ID (Нетворксеттингстипе)

Содержит значение идентификатора GUID, определяющее сетевой профиль.

``` syntax
<xs:element name="Id"
    type="guidType"
    minOccurs="0"
 />
```

Элемент **ID** определяется сложным типом [**нетворксеттингстипе**](taskschedulerschema-networksettingstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                            | Унаследован от                                                                       | Описание                                                                                                                                                                                                                                                                                                        |
|----------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Нетворксеттингс (Сеттингстипе)**](taskschedulerschema-networksettings-settingstype-element.md) | [**нетворксеттингстипе**](taskschedulerschema-networksettingstype-complextype.md) | Содержит параметры, используемые службой планировщик задач для получения сетевого профиля. Служба планировщик задач проверяет доступность этой сети, если для элемента [**рунонлифнетворкаваилабле**](taskschedulerschema-runonlyifnetworkavailable-settingstype-element.md) задано значение **true**.<br/> |



## <a name="remarks"></a>Remarks

Сведения о разработке на языке C++ см. в разделе [**свойство ID объекта инетворксеттингс**](/windows/desktop/api/taskschd/nf-taskschd-inetworksettings-get_id).

Сведения о разработке сценариев см. в разделе [**NetworkSettings.ID**](networksettings-id.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





