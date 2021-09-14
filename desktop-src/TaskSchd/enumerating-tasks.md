---
title: Перечисление задач
description: Планировщик задач 1,0 предоставляет объект перечисления для перечисления задач в папке «Назначенные задания».
ms.assetid: ccd140a1-06f6-4e6b-afa6-f7ac9b9ff904
keywords:
- Перечисление задач планировщик задач
- Перечисление задач планировщик задач, описание
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 81dda98cf40bc1ea360d20bcf13084faa692aa22
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056622"
---
# <a name="enumerating-tasks"></a>Перечисление задач

Планировщик задач 1,0 предоставляет объект перечисления для перечисления задач в [*папке «Назначенные задания*](s.md)».

> [!Note]  
> на компьютере Windows Server 2003, Windows XP или Windows 2000 для создания, отслеживания или управления задачами на компьютере Windows vista некоторые операции должны выполняться на компьютере Windows vista. Дополнительные сведения см. в разделе [Задачи](tasks.md).

 

## <a name="using-the-enumeration-object"></a>Использование объекта перечисления

Интерфейс [**иенумворкитемс**](/windows/desktop/api/Mstask/nn-mstask-ienumworkitems) этого объекта предоставляет методы для перечисления задач в папке, сброса последовательности перечисления до начала списка, пропуска задач и создания копии текущего объекта перечисления для последующего использования.

Сведения о перечислении задач в папке «запланированные задания» см. в разделе [**иенумворкитемс:: Next**](/windows/desktop/api/Mstask/nf-mstask-ienumworkitems-next).

Дополнительные сведения о сбросе перечисления в начало списка см. в разделе [**иенумворкитемс:: Reset**](/windows/desktop/api/Mstask/nf-mstask-ienumworkitems-reset).

Дополнительные сведения о пропуске задач см. в разделе [**иенумворкитемс:: Skip**](/windows/desktop/api/Mstask/nf-mstask-ienumworkitems-skip).

Сведения о создании копии текущего объекта перечисления см. в разделе [**иенумворкитемс:: Clone**](/windows/desktop/api/Mstask/nf-mstask-ienumworkitems-clone).

Пример перечисления задач в папке «запланированные задания» см. в разделе [Пример перечисления задач](enumerating-tasks-example.md).

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Сведения о задаче планировщик задач 1,0](task-scheduler-1-0-task-informatation.md)
</dt> </dl>

 

 




