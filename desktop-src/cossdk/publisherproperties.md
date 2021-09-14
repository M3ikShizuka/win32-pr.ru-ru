---
description: Содержит объект для каждого свойства издателя родительской коллекции Субскриптионсфоркомпонент.
ms.assetid: 7699c258-ca11-4652-b2f7-b2f2307c01fc
title: Коллекция Публишерпропертиес
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- PublisherProperties
api_type:
- COM
api_location: ''
ms.openlocfilehash: bdab3e8143ea3d35d07adb5caa73639fcb568cd1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056141"
---
# <a name="publisherproperties-collection"></a>Коллекция Публишерпропертиес

Содержит объект для каждого свойства издателя родительской коллекции [**субскриптионсфоркомпонент**](subscriptionsforcomponent.md) .

Эта коллекция поддерживает методы [**Add**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-add) и [**Remove**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-remove) объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) .

## <a name="members"></a>Элементы

Коллекция **публишерпропертиес** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) , но не содержит дополнительных элементов.

## <a name="related-collections"></a>Связанные коллекции

Можно переходить от этой коллекции к любой из следующих коллекций:

-   [**ErrorInfo**](errorinfo.md)
-   [**PropertyInfo**](propertyinfo.md)
-   [**релатедколлектионинфо**](relatedcollectioninfo.md)

Вы можете переходить к этой коллекции из следующих коллекций:

-   [**субскриптионсфоркомпонент**](subscriptionsforcomponent.md)

## <a name="properties"></a>Свойства

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



 

## <a name="see-also"></a>См. также:

<dl> <dt>

[Коллекции администрирования COM+](com--administration-collections.md)
</dt> </dl>

 

 
