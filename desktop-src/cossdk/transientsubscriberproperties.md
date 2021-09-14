---
description: Содержит объект для каждого свойства подписчика для родительской коллекции Трансиентсубскриптионс. Временные подписки можно создавать на лету для запуска экземпляров объектов, и они исчезают при уничтожении объекта.
ms.assetid: b4f003b0-db9d-45f1-a57d-3e4d321289ca
title: Коллекция Трансиентсубскриберпропертиес
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- TransientSubscriberProperties
api_type:
- COM
api_location: ''
ms.openlocfilehash: 17f89638efe232f2cdf06e1206f74a0df44601b2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347470"
---
# <a name="transientsubscriberproperties-collection"></a>Коллекция Трансиентсубскриберпропертиес

Содержит объект для каждого свойства подписчика для родительской коллекции [**трансиентсубскриптионс**](transientsubscriptions.md) . Временные подписки можно создавать на лету для запуска экземпляров объектов, и они исчезают при уничтожении объекта.

Эта коллекция поддерживает методы [**Add**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-add) и [**Remove**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-remove) объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) .

## <a name="members"></a>Элементы

Коллекция **трансиентсубскриберпропертиес** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) , но не содержит дополнительных элементов.

## <a name="related-collections"></a>Связанные коллекции

Можно переходить от этой коллекции к любой из следующих коллекций:

-   [**ErrorInfo**](errorinfo.md)
-   [**PropertyInfo**](propertyinfo.md)
-   [**релатедколлектионинфо**](relatedcollectioninfo.md)

Вы можете переходить к этой коллекции из следующих коллекций:

-   [**трансиентсубскриптионс**](transientsubscriptions.md)

## <a name="properties"></a>Элемент Property

Объект [**комадминкаталогобжект**](comadmincatalogobject.md) в коллекции поддерживает следующие свойства:

-   [имя](#name);
-   [Значение](#value)

### <a name="name"></a>Имя



| Ввод | Значение |
|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Описание    | Имя свойства. Лишние пробелы в начале и конце строки удаляются. Это свойство возвращается при вызове метода свойства [**Key**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_key) или [**Name**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_name) для объекта этой коллекции. |
| Access         | Флагом writeonce                                                                                                                                                                                                                                                              |
| Тип           | Строка                                                                                                                                                                                                                                                                 |
| По умолчанию        | "Создать свойство"                                                                                                                                                                                                                                                         |
| Минимальная система | Windows 2000                                                                                                                                                                                                                                                           |



 

### <a name="value"></a>Значение



| Ввод | Значение |
|----------------|---------------------------|
| Описание    | Значение для свойства. |
| Access         | ReadWrite                 |
| Тип           | Variant                   |
| По умолчанию        | Недоступно                       |
| Минимальная система | Windows 2000              |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коллекции администрирования COM+](com--administration-collections.md)
</dt> </dl>

 

 
