---
title: Совместное использование списков вывода
description: При создании контекста отрисовки он имеет свой собственный список отображения.
ms.assetid: 8ace5684-a27b-4d6e-a80b-58a0b7064879
keywords:
- OpenGL на Windows, совместное использование списков вывода
- Общий доступ списки дисплеев OpenGL
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 934789f3de00e6e0be451fc441416dfcbaa057b0b58b224fc57021db31575e71
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119776634"
---
# <a name="sharing-display-lists"></a>Совместное использование списков вывода

При создании контекста отрисовки он имеет свой собственный список отображения. Функция [**вглшарелистс**](/windows/desktop/api/wingdi/nf-wingdi-wglsharelists) позволяет контексту отрисовки совместно использовать пространство списка другого контекста визуализации. Любое количество контекстов отрисовки может совместно использовать одно пространство отображения.

 

 




