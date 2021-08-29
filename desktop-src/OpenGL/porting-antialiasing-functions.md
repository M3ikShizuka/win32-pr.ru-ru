---
title: Перенос функций сглаживания
description: Перенос функций сглаживания
ms.assetid: 7f79f0fa-4a08-4678-bc73-8611e8d9e91a
keywords:
- Перенос GL в ГК, сглаживание
- Перенос из ДИАФРАГМы в ГК, сглаживание
- перенос в OpenGL из IRI GL, сглаживание
- Перенос по стандарту OpenGL из IRI GL, сглаживание
- сглаживание
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 130fcf19efd3cd8f1082439bda1bd9c9702c8df7ea41cbe7655828a92e6cc9f4
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119777244"
---
# <a name="porting-antialiasing-functions"></a>Перенос функций сглаживания

В OpenGL режим подточки всегда включен, следовательно **, функция IRI** GL (**true**) не требуется и не имеет эквивалента OpenGL. В следующих разделах описаны аспекты переноса кода для сглаживания в ГК.

-   [Перенос кода смешения](porting-blending-code.md)
-   [Перенос тестовых функций афунктион](porting-afunction-test-functions.md)
-   [Использование функций сглаживания](using-antialiasing-functions.md)

 

 




