---
title: Интерфейс Ивмдрмпровидер
description: интерфейс ивмдрмпровидер предоставляет метод, создающий другие объекты расширенных api клиента DRM Microsoft Windows Media. вы можете получить указатель на экземпляр этого интерфейса, вызвав функцию вмдрмкреатепровидер.
ms.assetid: bcd346e3-a79f-49a8-b5f9-b9ae8b54527a
keywords:
- Формат Windows Media в интерфейсе Ивмдрмпровидер
- Ивмдрмпровидер интерфейса Windows Media Format, описание
topic_type:
- apiref
api_name:
- IWMDRMProvider
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: bfe08a00d94914744f184ac4d0409fed24701985740006841f1d178cc39273e8
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119930124"
---
# <a name="iwmdrmprovider-interface"></a>Интерфейс Ивмдрмпровидер

интерфейс **ивмдрмпровидер** предоставляет метод, который создает другие объекты расширенных api-интерфейсов клиента DRM Microsoft Windows Media.

Указатель на экземпляр этого интерфейса можно получить, вызвав функцию [**вмдрмкреатепровидер**](wmdrmcreateprovider.md) . Чтобы получить указатель на экземпляр этого интерфейса, который может создавать защищенные объекты, необходимо вызвать функцию [**вмдрмкреатепротектедпровидер**](wmdrmcreateprotectedprovider.md) .

## <a name="members"></a>Элементы

Интерфейс **ивмдрмпровидер** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **Ивмдрмпровидер** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **ивмдрмпровидер** содержит следующие методы.



| Метод                                              | Описание                                                                                          |
|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------|
| [**CreateObject**](iwmdrmprovider-createobject.md) | Извлекает указатель на указанный интерфейс, создавая реализующий объект при необходимости.<br/> |



 

## <a name="see-also"></a>См. также

<dl> <dt>

[**Интерфейсы**](drm-interfaces.md)
</dt> </dl>

 

