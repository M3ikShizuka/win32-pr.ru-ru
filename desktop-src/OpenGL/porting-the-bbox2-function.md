---
title: Перенос функции bbox2
description: Для функции IRI GL bbox2 не существует эквивалента OpenGL.
ms.assetid: 2d8082bf-c2c3-41d9-9bf7-b4ac2fdefbd6
keywords:
- Перенос GL в ГК, функция bbox2
- Перенос из IRI GL, функция bbox2
- перенос в OpenGL из IRI GL, функция bbox2
- Перенос по стандарту OpenGL из IRI GL, функция bbox2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 21060b8a11ccd6c44297c8b533bca98d79cc00f7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127348335"
---
# <a name="porting-the-bbox2-function"></a>Перенос функции bbox2

Для функции IRI GL **bbox2** не существует эквивалента OpenGL.

**Перенос кода, содержащего функции bbox2**

1.  Создайте новый список дисплеев (OpenGL), содержащий все в эквивалентном списке дисплеев ДИАФРАГМы, за исключением вызова **bbox2**.
2.  используйте соответствующий код Windows, чтобы нарисовать прямоугольник того же размера, что и для диафрагмы **ббокс** GL.

 

 




