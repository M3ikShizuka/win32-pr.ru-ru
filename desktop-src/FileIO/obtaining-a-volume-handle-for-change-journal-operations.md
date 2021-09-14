---
description: 'Чтобы получить маркер для тома, который будет использоваться с операциями с журналом изменений (USN), вызовите функцию CreateFile с параметром Лпфиленаме, для которого задана строка следующего вида: \\ \\ . \\ X.'
ms.assetid: a4f4dac5-76fd-4e9e-a71e-665684840d74
title: Получение маркера тома для операций журнала изменений
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e8036fc642de52aa2d7f9bab66dd2e380dcc070c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057851"
---
# <a name="obtaining-a-volume-handle-for-change-journal-operations"></a>Получение маркера тома для операций журнала изменений

Чтобы получить маркер для тома, который будет использоваться с операциями с журналом изменений (USN), вызовите функцию [**CreateFile**](/windows/desktop/api/FileAPI/nf-fileapi-createfilea) с параметром *лпфиленаме* , для которого задана строка следующего вида: \\ \\ . \\ *X*:

Обратите внимание, что *X* — это буква, идентифицирующая диск, на котором отображается том NTFS.

Если у тома нет буквы диска, используйте синтаксис, описанный в разделе [именование тома](naming-a-volume.md).

 

 



