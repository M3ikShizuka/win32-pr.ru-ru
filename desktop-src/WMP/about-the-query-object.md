---
title: Сведения об объекте Query
description: Сведения об объекте Query
ms.assetid: 41488036-bdcf-4fe6-8f7e-f0897157d3d9
keywords:
- проигрыватель Windows Media, объект Query
- объектная модель проигрыватель Windows Media, объект Query
- Объектная модель, объект Query
- проигрыватель Windows Media элемент управления ActiveX, объект Query
- элемент управления ActiveX, объект Query
- проигрыватель Windows Media мобильный ActiveX элемент управления, объект Query
- проигрыватель Windows Media Мобильные запросы, объект Query
- Объект запроса
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 54a26f60c38e053b91c7e56f5cbd7ccaf2ba0fe2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126890216"
---
# <a name="about-the-query-object"></a>Сведения об объекте Query

Объект **Query** представляет составной запрос. Создайте новый пустой объект **запроса** , вызвав *медиаколлектион*. **createQuery**. После создания объекта **запроса** можно вызвать **аддкондитион** , чтобы добавить условие в составной запрос. Каждый последующий вызов **аддкондитион** добавляет новое условие к существующему запросу с помощью логики и.

Например, предположим, что требуется создать запрос, представляющий все цифровые мультимедийные файлы, где **WM/жанр** равен «джаз», а **Автор** содержит «Джим». можно создать составной запрос для представления этих условий с помощью следующего JScript кода:


```C++
// Create the query object.
var Query = player.mediaCollection.createQuery();

// Add the conditions.
Query.addCondition("WM/Genre", "Equals", "Jazz");
Query.addCondition("Author", "Contains", "Jim");
```



Чтобы добавить условие в составной запрос с помощью или логики, необходимо вызвать метод **Query. бегиннекстграуп**. Этот метод сигнализирует, что предыдущая группа условий завершена и что следующий вызов **аддкондитион** представляет начало новой группы условий.

Например, чтобы создать запрос, представляющий все цифровые мультимедийные файлы, в которых **WM/жанр** равен «джаз», а **Author** содержит «Джим» или « **Author** » содержит «Дейв», можно использовать следующий пример кода:


```C++
// Create the query object.
var Query = player.mediaCollection.createQuery();

// Add the conditions.
Query.addCondition("WM/Genre", "Equals", "Jazz");
Query.addCondition("Author", "Contains", "Jim");

// Start the next condition group. This group will be
// combined with the previous group using a logical OR operation.
Query.beginNextGroup();

// Add the conditions.
Query.addCondition("WM/Genre", "Equals", "Jazz");
Query.addCondition("Author", "Contains", "Dave");
```



Чтобы выполнить составной запрос, вызовите метод **медиаколлектион. жетплайлистбикуери**.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Медиаколлектион. Жетплайлистбикуери**](mediacollection-getplaylistbyquery.md)
</dt> <dt>

[**Объектная модель проигрывателя для языков сценариев**](player-object-model-for-scripting-languages.md)
</dt> <dt>

[**Объект запроса**](query-object.md)
</dt> </dl>

 

 




