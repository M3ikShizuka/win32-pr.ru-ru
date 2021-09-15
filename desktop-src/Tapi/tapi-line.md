---
description: Класс устройств TAPI/Line состоит из всех устройств линии. Доступ к этим устройствам осуществляется с помощью функций линии TAPI.
ms.assetid: 2215b10b-e410-462c-8cf9-42f3e688e82e
title: TAPI/Line
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 928cfa6144e9a701d6462519d2aa9d590a54a511
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469779"
---
# <a name="tapiline"></a>TAPI/Line

Класс устройств TAPI/Line состоит из всех устройств линии. Доступ к этим устройствам осуществляется с помощью функций линии TAPI.

Функция [**линежетид**](/windows/desktop/api/Tapi/nf-tapi-linegetid) заполняет структуру [**варстринг**](/windows/desktop/api/Tapi/ns-tapi-varstring) , устанавливая элемент **ДВСТРИНГФОРМАТ** в \_ двоичное значение STRINGFORMAT и добавляя этот дополнительный элемент.

``` syntax
DWORD dwDeviceI;  // line device identifier
```

Элемент **двдевицеид** — это идентификатор устройства линии, связанного с маркером линии, заданным параметром [**линежетид**](/windows/desktop/api/Tapi/nf-tapi-linegetid).

Функция [**фонежетид**](/windows/desktop/api/Tapi/nf-tapi-phonegetid) также заполняет структуру [**варстринг**](/windows/desktop/api/Tapi/ns-tapi-varstring) , настроив **двстрингформат** на STRINGFORMAT \_ binary и добавляя этот дополнительный элемент:

``` syntax
DWORD adwDeviceIds[];  // array of line device identifiers
```

Элемент **адвдевицеидс** — это массив, содержащий идентификаторы устройств всех устройств линий, связанных с телефонным устройством. Если связанных устройств нет, [**фонежетид**](/windows/desktop/api/Tapi/nf-tapi-phonegetid) ВОЗВРАЩАЕТ \_ значение фонирр инвалдевицекласс.

 

 



