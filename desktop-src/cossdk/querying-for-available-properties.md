---
description: Запрос доступных свойств
ms.assetid: 9acf10cd-19a8-4542-8078-3e4ee275d4d5
title: Запрос доступных свойств
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 22238e04404d2b88efa81ce98d0b0fb0e09d245f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566814"
---
# <a name="querying-for-available-properties"></a>Запрос доступных свойств

При написании средства администрирования общего назначения вам, скорее всего, придется написать подпрограммы для настройки свойств в полной общей настройке. Для этого существует средство, которое позволяет динамически запрашивать свойства, доступные для элементов в любой заданной коллекции.

Коллекция [**PropertyInfo**](propertyinfo.md) доступна из любой коллекции, которую вы можете удерживать. Коллекция **PropertyInfo** содержит элемент для каждого доступного свойства. Можно перечислить эти элементы, чтобы определить, доступно ли данное свойство.

Коллекцию [**PropertyInfo**](propertyinfo.md) можно получить из любой коллекции, которую вы удерживаете, используя метод [**IsCollection**](/windows/desktop/api/ComAdmin/nf-comadmin-icomadmincatalog-getcollection) для объекта [**комадминкаталогколлектион**](comadmincatalogcollection.md) , и оставить второй параметр пустым, где обычно указывается свойство ключа родительского элемента.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Получение и задание свойств](getting-and-setting-properties.md)
</dt> <dt>

[Взаимозависимости между свойствами](interdependencies-between-properties.md)
</dt> <dt>

[Сохранение или Отмена изменений](saving-or-discarding-changes.md)
</dt> </dl>

 

 



