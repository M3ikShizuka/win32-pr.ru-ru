---
description: Запросы к доступным связанным коллекциям
ms.assetid: 9c7d2a01-5dc3-4d35-b938-f1d0525a8286
title: Запросы к доступным связанным коллекциям
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0203df5bb7b5bf89396d5687dc28b19e9b183d56
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127457689"
---
# <a name="querying-for-available-related-collections"></a>Запросы к доступным связанным коллекциям

При написании средства администрирования общего назначения, скорее всего, потребуется написать подпрограммы для навигации по всей иерархии коллекции. Для этого в COM+ есть средство, которое позволяет динамически запрашивать связанные коллекции, доступные из любой заданной коллекции.

Коллекция [**релатедколлектионинфо**](relatedcollectioninfo.md) доступна из любой коллекции, которая может храниться, и содержит элемент для каждой доступной связанной коллекции. Можно перечислить эти элементы, чтобы определить, доступна ли данная коллекция.

Коллекцию [**релатедколлектионинфо**](relatedcollectioninfo.md) можно получить из любой коллекции, которую вы удерживаете, с помощью метода [**IsCollection**](/windows/desktop/api/ComAdmin/nf-comadmin-icomadmincatalog-getcollection) объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) . Второй параметр остается пустым, где обычно указывается свойство ключа родительского элемента.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Навигация по иерархии коллекции COM+](navigating-the-com--collection-hierarchy.md)
</dt> <dt>

[Заполнение коллекций COM+](populating-com--collections.md)
</dt> <dt>

[Получение коллекций в каталоге COM+](retrieving-collections-on-the-com--catalog.md)
</dt> </dl>

 

 



