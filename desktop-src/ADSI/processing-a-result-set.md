---
title: Обработка результирующего набора
description: Результирующий набор возвращается в виде последовательности строк.
ms.assetid: e0949c1c-a31a-440a-ae10-2934ffeb7128
ms.tgt_platform: multiple
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 41ad422494fd2d384b612989e9e36cec7110e021
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174603"
---
# <a name="processing-a-result-set"></a>Обработка результирующего набора

Результирующий набор возвращается в виде последовательности строк. Каждая строка может не содержать заданный атрибут. при использовании поставщика OLE DB результирующий набор будет похож на нормальный SQL результирующий набор. При использовании ADO для запроса объект [ADODB. Объект Recordset](/sql/ado/reference/ado-api/recordset-object-ado?view=sql-server-ver15) используется для обхода результирующего набора. [**IDirectorySearch**](/windows/desktop/api/Iads/nn-iads-idirectorysearch) (доступно только на языках, поддерживающих привязки vtable) содержит элементы для перемещения курсора строки и проверки значений свойств в заданной строке. Кроме того, можно использовать [**идиректорйобжект**](/windows/desktop/api/Iads/nn-iads-idirectoryobject) для получения и задания свойств.

 

 