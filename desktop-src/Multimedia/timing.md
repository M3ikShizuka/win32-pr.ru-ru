---
title: время (Windows мультимедиа)
description: Временные свойства
ms.assetid: 9ab284c7-eebc-4b44-b9e1-cc95efde22c1
keywords:
- Дравдиб, время
- Функция Дравдибтиме
- Дравдиб, отладка
- Отладка Дравдиб
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: adddd43ff5067d08334a40f2e52e79109c8a8bb7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127260576"
---
# <a name="timing-windows-multimedia"></a>время (Windows мультимедиа)

В рамках отладки приложения можно получить сведения о количестве времени, необходимого для выполнения повторяющихся операций Дравдиб. Функция [**дравдибтиме**](/windows/desktop/api/Vfw/nf-vfw-drawdibtime) возвращает сведения о времени для следующих операций:

-   Рисование точечного рисунка
-   Распаковка точечного рисунка
-   Сглаживание точечного рисунка
-   Растяжение растрового изображения
-   Передача точечного рисунка с помощью функции [**BitBlt**](/windows/desktop/api/wingdi/nf-wingdi-bitblt)
-   Передача точечного рисунка с помощью функции [**стретчдибитс**](/windows/desktop/api/wingdi/nf-wingdi-stretchdibits)

После получения набора значений [**дравдибтиме**](/windows/desktop/api/Vfw/nf-vfw-drawdibtime) сбрасывает количество и значение для каждой операции.

Функция [**дравдибтиме**](/windows/desktop/api/Vfw/nf-vfw-drawdibtime) доступна только в отладочной версии функций дравдиб.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Рендеринг изображений](image-rendering.md)
</dt> </dl>

 

 
