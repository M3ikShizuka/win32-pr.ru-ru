---
description: Атрибут Time указывает время, когда параметр принимает новое значение относительно начала перехода или воздействия.
ms.assetid: bb478215-cbd5-4fea-9d88-a1f2b002f3da
title: Атрибут времени
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c4d4ed72cc76935f68973634643fc5dbdf719b150f096ec43e1ace56881f0c26
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120083654"
---
# <a name="time-attribute"></a>Атрибут времени

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`time`Атрибут задает время, когда параметр принимает новое значение относительно начала перехода или воздействия.

## <a name="possible-values"></a>Возможные значения

Должен быть строкой формата *чч: мм: СС. FF* , где *чч* = ч, *мм* = минуты, *SS* = секунды и *FF* = доли секунды. Пример: 1:04:30.512. Начальные единицы можно опустить. Например, допустимыми являются 3:00 (три минуты) и 45 (45 секунд).

## <a name="applies-to"></a>Применяется к

[**в**](at-element.md), [ **Линейная**](linear-element.md)

## <a name="see-also"></a>См. также

<dl> <dt>

[Атрибуты КСТЛ](xtl-attributes.md)
</dt> </dl>

 

 



