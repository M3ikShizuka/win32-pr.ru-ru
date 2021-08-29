---
description: Распределитель памяти
ms.assetid: 2dc055a2-b77a-443d-b602-d9636cbe4db3
title: Распределитель памяти
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9346cf35e9383ff79e3dc5dafe54c0857a3f6f8818d9d137ae92bd1e6f98977d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119584154"
---
# <a name="memory-allocator"></a>Распределитель памяти

Объект распределителя памяти выделяет буферы для образцов мультимедиа. Фильтры могут использовать этот объект для выделения буферов общей памяти; Однако фильтр с особыми требованиями также может реализовать собственный объект распределителя памяти. Создайте этот объект, вызвав **CoCreateInstance**.



| Метка | Значение |
|------------------|----------------------------------------|
| Идентификатор класса | \_МЕМОРЯЛЛОКАТОР CLSID                 |
| Интерфейсы       | [**имемаллокатор**](/windows/desktop/api/Strmif/nn-strmif-imemallocator) |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Объект](directshow-objects.md)
</dt> </dl>

 

 



