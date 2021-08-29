---
description: Содержит список серверных компьютеров в кластере приложений. Он содержит объект для каждого сервера.
ms.assetid: 8722080a-cf95-4c29-9eb7-99c6df93611f
title: Коллекция Аппликатионклустер
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ApplicationCluster
api_type:
- COM
api_location: ''
ms.openlocfilehash: 852f6f04147489336622a5c13e447bcb4fbfd7e20f580edcb5da8bdfadaa5e7a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119991950"
---
# <a name="applicationcluster-collection"></a>Коллекция Аппликатионклустер

Содержит список серверных компьютеров в кластере приложений. Он содержит объект для каждого сервера. Это коллекция верхнего уровня.

Кластер приложений определяется в целях службы балансировки нагрузки компонентов (распределения загрузки). Для использования коллекции кластеров приложений на компьютере должна быть установлена служба распределения загрузки.

Вы назначаете маршрутизатор в кластере приложений с помощью свойства IsCollection в объекте коллекции [**локалкомпутер**](localcomputer.md) , и вы указываете, что заданный компонент должен быть сбалансирован с помощью свойства лоадбаланЦингсуппортед в объекте коллекции [**компонентов**](components.md) .

Эта коллекция поддерживает методы [**Add**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-add) и [**Remove**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogcollection-remove) объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) .

## <a name="members"></a>Элементы

Коллекция **аппликатионклустер** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) , но не содержит дополнительных элементов.

## <a name="related-collections"></a>Связанные коллекции

Можно переходить от этой коллекции к любой из следующих коллекций:

-   [**ErrorInfo**](errorinfo.md)
-   [**PropertyInfo**](propertyinfo.md)
-   [**релатедколлектионинфо**](relatedcollectioninfo.md)

Вы можете переходить к этой коллекции из следующих коллекций:

-   [**Корневой**](root.md)

## <a name="properties"></a>Свойства

Объект [**комадминкаталогобжект**](comadmincatalogobject.md) в коллекции поддерживает следующие свойства:

-   [Имя](#name)

### <a name="name"></a>Имя



| Ввод | Значение |
|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Описание    | Имя сервера. Лишние пробелы в начале и конце строки удаляются. Это свойство возвращается при вызове метода свойства [**Key**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_key) или [**Name**](/windows/desktop/api/ComAdmin/nf-comadmin-icatalogobject-get_name) для объекта этой коллекции. |
| Доступ         | Флагом writeonce                                                                                                                                                                                                                                                            |
| Тип           | Строка                                                                                                                                                                                                                                                               |
| По умолчанию        | "Новый компьютер"                                                                                                                                                                                                                                                       |
| Минимальная система | Windows 2000                                                                                                                                                                                                                                                         |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коллекции администрирования COM+](com--administration-collections.md)
</dt> </dl>

 

 
