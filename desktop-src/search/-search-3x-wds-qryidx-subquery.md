---
description: сведения о аргументе вложенного запроса в Windows поиске. Вложенный запрос — это сохраненный файл поиска, который можно использовать в качестве фильтра для нового запроса.
ms.assetid: a92c774f-310b-4c40-be1c-0c2b0cac907b
title: аргумент вложенного запроса (поиск Windows)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 93b23028d0bddcc674714f51f8b31883052431bd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363268"
---
# <a name="subquery-argument-windows-search"></a>аргумент вложенного запроса (поиск Windows)

Вложенный запрос — это сохраненный файл поиска ( \* . Search-MS), который можно использовать в качестве фильтра для нового запроса. Результаты вложенного запроса используются в качестве источника для нового запроса. Например, предположим, что имеется несколько сохраненных файлов поиска, ограничивающих запрос по списку рассылки электронной почты: мидепартмент. Search-MS, TeamProject. Search-MS и корпоратевиде. Search-MS. Использование `subquery` аргумента позволяет ограничить поиск по электронной почте любым из сохраненных поисков.

Этот раздел организован следующим образом:

-   [Пример](#example)
-   [Связанные темы](#related-topics)

## <a name="example"></a>Пример


```
 search-ms:query=vacation&subquery=mydepartment.search-ms
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Начало работы с Parameter-Valueными аргументами](getting-started-with-parameter-value-arguments.md)
</dt> <dt>

[Аргументы идентификатора языкового стандарта](-search-3x-wds-qryidx-localeidentifiers.md)
</dt> <dt>

[Переданный аргумент](-search-3x-wds-qryidx-crumb.md)
</dt> <dt>

[Аргумент СИНТАКСИСа](-search-3x-wds-qryidx-syntaxargument.md)
</dt> <dt>

[СТАККЕДБИ, аргумент](-search-3x-wds-qryidx-stackedby.md)
</dt> </dl>

 

 



