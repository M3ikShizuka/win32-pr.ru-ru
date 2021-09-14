---
title: Fragments
description: Fragments
ms.assetid: bc400251-32c4-4477-ba0c-a0046fe85327
keywords:
- OpenGL, фрагменты
- Конвейер обработки OpenGL, фрагменты
- фрагменты OpenGL
- фрамебуфферс, фрагменты, изменяющие Пиксели
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 00e2b4c2dc36e24c4fd9baa82b28fa4d336f69b5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064971"
---
# <a name="fragments"></a>Fragments

Фрагмент, созданный путем растрирования, изменяет соответствующий пиксель в буфера кадров только в том случае, если он проходит следующие тесты:

-   [Тестирование владения пикселями](pixel-ownership-test.md)
-   [Ножницное тестирование](scissor-test.md)
-   [Альфа-тест](alpha-test.md)
-   [Тест набора элементов](stencil-test.md)
-   [Тест буфера глубины](depth-buffer-test.md)

При передаче данные фрагмента могут заменить существующие значения буфера кадров или объединить его с существующими данными в буфера кадров в зависимости от состояния определенных режимов. Фрагмент можно объединить с данными в буфера кадров, выполнив следующие действия.

-   [Смешения](blending.md)
-   [Сглаживания](dithering.md)
-   [Логические операции](logical-operations.md)

 

 




