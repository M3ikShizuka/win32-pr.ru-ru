---
title: Методы (IInertiaProcessor)
description: В этом разделе содержатся методы для интерфейса IInertiaProcessor.
ms.assetid: e4acfcac-06c1-42a5-9722-4534a4492ab8
keywords:
- Windows Сенсорный ввод, интерфейс IInertiaProcessor
- Windows Сенсорный ввод, методы интерфейса
- инерция, интерфейс IInertiaProcessor
- Интерфейс IInertiaProcessor, методы
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3cb5c03039c09ef1435fcddd4782a466fff3aa179d57e5abb3887fa9212ca753
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119881444"
---
# <a name="methods-iinertiaprocessor"></a>Методы (IInertiaProcessor)

В этом разделе содержатся методы для интерфейса [**IInertiaProcessor**](/windows/desktop/api/manipulations/nn-manipulations-iinertiaprocessor) .



| Метод                                                 | Описание                                                                                                                                                                                                                |
|--------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Перезапуск**](/windows/desktop/api/manipulations/nf-manipulations-iinertiaprocessor-reset)               | Инициализирует процессор с начальной меткой времени и перезапускает инерцию.                                                                                                                                                    |
| [**Процесс**](/windows/desktop/api/manipulations/nf-manipulations-iinertiaprocessor-process)           | Выполняет вычисления для текущего такта и может вызвать событие **Дельта** или **Completed** в зависимости от того, завершено ли экстраполяция. Если экстраполяция завершается в предыдущем такте, метод является оператором No-Op. |
| [**процесстиме**](/windows/desktop/api/manipulations/nf-manipulations-iinertiaprocessor-processtime)   | Выполняет вычисления для заданного такта и может вызвать событие **Дельта** или **Completed** в зависимости от того, завершено ли экстраполяция.                                                                        |
| [**Завершить**](/windows/desktop/api/manipulations/nf-manipulations-iinertiaprocessor-complete)         | Завершает текущую манипуляцию и останавливает инерцию в обработчике инерции.                                                                                                                                              |
| [**комплететиме**](/windows/desktop/api/manipulations/nf-manipulations-iinertiaprocessor-completetime) | Завершает текущую обработку в заданном такте, останавливает инерцию в обработчике инерции и создает событие ManipulationCompleted.                                                                                   |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**IInertiaProcessor**](/windows/desktop/api/manipulations/nn-manipulations-iinertiaprocessor)
</dt> </dl>

 

 




