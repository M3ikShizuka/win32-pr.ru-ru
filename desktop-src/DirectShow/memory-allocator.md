---
description: Распределитель памяти
ms.assetid: 2dc055a2-b77a-443d-b602-d9636cbe4db3
title: Распределитель памяти
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4e2412adb78be18ac8c14eb4706624424f97ff13
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065629"
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

 

 



