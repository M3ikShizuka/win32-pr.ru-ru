---
description: Указывает приложения, содержащиеся в каждой секции.
ms.assetid: 264a35fd-ba71-4ae9-908a-24a72167c26b
title: Коллекция partitions
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Partitions
api_type:
- COM
api_location: ''
ms.openlocfilehash: 2f7ba43cbfd33736c9997adb4c312e044cf28e6e
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122882525"
---
# <a name="partitions-collection"></a>Коллекция partitions

Указывает приложения, содержащиеся в каждой секции.

Эта коллекция поддерживает методы [**Add**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-add) и [**Remove**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-remove) объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) .

## <a name="members"></a>Элементы

Коллекция **partitions** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) , но не содержит дополнительных элементов.

## <a name="related-collections"></a>Связанные коллекции

Можно переходить от этой коллекции к любой из следующих коллекций:

-   [**Приложения**](applications.md)
-   [**ErrorInfo**](errorinfo.md)
-   [**PropertyInfo**](propertyinfo.md)
-   [**релатедколлектионинфо**](relatedcollectioninfo.md)
-   [**ролесфорпартитион**](rolesforpartition.md)

Вы можете переходить к этой коллекции из следующих коллекций:

-   [**Root**](root.md)

## <a name="properties"></a>Свойства

Объект [**комадминкаталогобжект**](comadmincatalogobject.md) в коллекции поддерживает следующие свойства:

-   [Поддержка изменений](#changeable)
-   [Предусмотрено](#deleteable)
-   [Описание](#description)
-   [ID](#partitions-collection)
-   [имя](#name);

### <a name="changeable"></a>Поддержка изменений



| Ввод | Значение |
|----------------|--------------------------------------------------|
| Описание    | Определяет, является ли секция изменяемой. |
| Access         | ReadWrite                                        |
| Тип           | Bool                                             |
| По умолчанию        | Верно                                             |
| Минимальная система | Windows Server 2003                              |



 

### <a name="deleteable"></a>Предусмотрено



| Ввод | Значение |
|----------------|---------------------------------------------------|
| Описание    | Определяет, можно ли удалить эту секцию. |
| Access         | ReadWrite                                         |
| Тип           | Bool                                              |
| По умолчанию        | Верно                                              |
| Минимальная система | Windows Server 2003                               |



 

### <a name="description"></a>Описание



| Ввод | Значение |
|----------------|---------------------------------------------------------------------|
| Описание    | Это свойство представляет описание, идентифицирующее секцию. |
| Access         | ReadWrite                                                           |
| Тип           | Строка                                                              |
| По умолчанию        | ""                                                                  |
| Минимальная система | Windows Server 2003                                                 |



 

### <a name="id"></a>ID



| Ввод | Значение |
|----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Описание    | Идентификатор GUID, представляющий секцию. Это свойство возвращается при вызове метода свойства [**ключа**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_key) для объекта этой коллекции. |
| Access         | Флагом writeonce                                                                                                                                                          |
| Тип           | Строка                                                                                                                                                             |
| По умолчанию        | &lt;Сформировано&gt;                                                                                                                                                  |
| Минимальная система | Windows Server 2003                                                                                                                                                |



 

### <a name="name"></a>Имя



| Ввод | Значение |
|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Описание    | Представляет имя секции. Лишние пробелы в начале и конце строки удаляются. Это свойство возвращается при вызове метода свойства [**Name**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_name) для объекта этой коллекции. |
| Access         | ReadWrite                                                                                                                                                                                                                              |
| Тип           | Строка                                                                                                                                                                                                                                 |
| По умолчанию        | "Создать секцию"                                                                                                                                                                                                                        |
| Минимальная система | Windows Server 2003                                                                                                                                                                                                                    |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коллекции администрирования COM+](com--administration-collections.md)
</dt> </dl>

 

 
