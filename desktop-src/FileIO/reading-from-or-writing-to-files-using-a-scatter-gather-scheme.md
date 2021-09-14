---
description: Описывает схему разбивки на части для чтения или записи несмежных фрагментов данных за одну операцию.
ms.assetid: ae5d83ca-f219-4fcc-ad06-bc242ba95372
title: Чтение или запись в файлы с помощью схемы Scatter-Gather
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5a7db31dd73dd0b498436548a867dd92ff248805
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057821"
---
# <a name="reading-from-or-writing-to-files-using-a-scatter-gather-scheme"></a>Чтение или запись в файлы с помощью схемы Scatter-Gather

Схема разбивки на части использует операционную систему для доставки в одной операции нескольких дискретных блоков данных (например, записей базы данных) из файла в отдельные несмежные буферы в памяти. Схема рассеивания также записывает данные из несмежных буферов за одну операцию.

Приложение может реализовать схему разбивки на области с помощью функций [**реадфилескаттер**](/windows/desktop/api/FileAPI/nf-fileapi-readfilescatter) и [**вритефилегасер**](/windows/desktop/api/FileAPI/nf-fileapi-writefilegather) .

 

 



