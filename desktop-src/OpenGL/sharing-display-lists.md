---
title: Совместное использование списков вывода
description: При создании контекста отрисовки он имеет свой собственный список отображения.
ms.assetid: 8ace5684-a27b-4d6e-a80b-58a0b7064879
keywords:
- OpenGL на Windows, совместное использование списков вывода
- Общий доступ списки дисплеев OpenGL
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 87d8d012e8e04455f76ca5d7bfe74229ac0b0ac8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057227"
---
# <a name="sharing-display-lists"></a>Совместное использование списков вывода

При создании контекста отрисовки он имеет свой собственный список отображения. Функция [**вглшарелистс**](/windows/desktop/api/wingdi/nf-wingdi-wglsharelists) позволяет контексту отрисовки совместно использовать пространство списка другого контекста визуализации. Любое количество контекстов отрисовки может совместно использовать одно пространство отображения.

 

 




