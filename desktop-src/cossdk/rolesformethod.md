---
description: Содержит объект для каждой роли, назначенной методу, к которому относится коллекция. Роли уже должны быть назначены на уровне приложения.
ms.assetid: 3a086163-e367-4dd1-996b-821b3e1111b2
title: Коллекция Ролесформесод
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- RolesForMethod
api_type:
- COM
api_location: ''
ms.openlocfilehash: c73ba5f7a14a5efc6711a65f211cd036e1c2a14d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126971213"
---
# <a name="rolesformethod-collection"></a>Коллекция Ролесформесод

Содержит объект для каждой роли, назначенной методу, к которому относится коллекция. Роли уже должны быть назначены на уровне приложения.

Эта коллекция поддерживает методы [**Add**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-add) и [**Remove**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-remove) объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) .

## <a name="members"></a>Элементы

Коллекция **ролесформесод** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) , но не содержит дополнительных элементов.

## <a name="related-collections"></a>Связанные коллекции

Можно переходить от этой коллекции к любой из следующих коллекций:

-   [**ErrorInfo**](errorinfo.md)
-   [**PropertyInfo**](propertyinfo.md)
-   [**релатедколлектионинфо**](relatedcollectioninfo.md)

Вы можете переходить к этой коллекции из следующих коллекций:

-   [**месодсфоринтерфаце**](methodsforinterface.md)

## <a name="properties"></a>Свойства

Объект [**комадминкаталогобжект**](comadmincatalogobject.md) в коллекции поддерживает следующие свойства:

-   [имя](#name);

### <a name="name"></a>Имя



| Ввод | Значение |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Описание    | Имя роли. Уже должна быть назначена приложению роли (отображается в коллекции ролей). Лишние пробелы в начале и конце строки удаляются. Это свойство возвращается при вызове метода свойства [**Key**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_key) или [**Name**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_name) для объекта этой коллекции. |
| Access         | Флагом writeonce                                                                                                                                                                                                                                                                                                                                           |
| Тип           | Строка                                                                                                                                                                                                                                                                                                                                              |
| По умолчанию        | "Создать роль"                                                                                                                                                                                                                                                                                                                                          |
| Минимальная система | Windows 2000                                                                                                                                                                                                                                                                                                                                        |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коллекции администрирования COM+](com--administration-collections.md)
</dt> </dl>

 

 
