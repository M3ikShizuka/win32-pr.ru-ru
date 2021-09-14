---
description: Windows использует указатель файла для наблюдения за чтением или записью байтов.
ms.assetid: 21c75d96-0357-422d-b12b-74c56f64ecf1
title: Размещение указателя на файл
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d6588a3d65e71c2180c4e9753e65cd94ed070d36
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057829"
---
# <a name="positioning-a-file-pointer"></a>Размещение указателя на файл

когда приложение вызывает [**CreateFile**](/windows/desktop/api/FileAPI/nf-fileapi-createfilea) для открытия файла в первый раз, Windows помещает [указатель файла](file-pointers.md) в начало файла. так как байты считываются из файла или записываются в файл, Windows изменяет указатель файла на число считанных или записанных байтов.

Приложение может поместить указатель файла в указанное смещение, вызвав [**SetFilePointer**](/windows/desktop/api/FileAPI/nf-fileapi-setfilepointer).

Функция [**SetFilePointer**](/windows/desktop/api/FileAPI/nf-fileapi-setfilepointer) может также использоваться для запроса текущей позиции указателя файла путем указания метода Move **файла \_ Current** и расстояния от нуля.

 

 



