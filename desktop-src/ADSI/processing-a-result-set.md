---
title: Обработка результирующего набора
description: Результирующий набор возвращается в виде последовательности строк.
ms.assetid: e0949c1c-a31a-440a-ae10-2934ffeb7128
ms.tgt_platform: multiple
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8481908f55ab6710a2a2b116b76331643f1798a3b7317cd858cee796a4831307
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119828394"
---
# <a name="processing-a-result-set"></a>Обработка результирующего набора

Результирующий набор возвращается в виде последовательности строк. Каждая строка может не содержать заданный атрибут. при использовании поставщика OLE DB результирующий набор будет похож на нормальный SQL результирующий набор. При использовании ADO для запроса объект [ADODB. Объект Recordset](/sql/ado/reference/ado-api/recordset-object-ado?view=sql-server-ver15) используется для обхода результирующего набора. [**IDirectorySearch**](/windows/desktop/api/Iads/nn-iads-idirectorysearch) (доступно только на языках, поддерживающих привязки vtable) содержит элементы для перемещения курсора строки и проверки значений свойств в заданной строке. Кроме того, можно использовать [**идиректорйобжект**](/windows/desktop/api/Iads/nn-iads-idirectoryobject) для получения и задания свойств.

 

 