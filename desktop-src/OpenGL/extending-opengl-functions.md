---
title: Расширение функций OpenGL
description: Библиотека OpenGL поддерживает несколько реализаций своих функций.
ms.assetid: 9eb08fd4-899a-4610-9491-d7f377a19b46
keywords:
- OpenGL на Windows, функции расширения
- функции расширения OpenGL
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7dcbb59aa15a9690ac05728548f0d8073a334a2e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461636"
---
# <a name="extending-opengl-functions"></a>Расширение функций OpenGL

Библиотека OpenGL поддерживает несколько реализаций своих функций. Функции расширения, поддерживаемые в одном контексте отрисовки, не обязательно поддерживаются в другом контексте отрисовки. Для данного контекста отрисовки в приложении, использующем функции расширения, используйте только адреса функций, возвращенные функцией [**вглжетпрокаддресс**](/windows/desktop/api/wingdi/nf-wingdi-wglgetprocaddress) .

 

 




