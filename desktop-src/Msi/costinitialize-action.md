---
description: Действие Костинитиализе инициирует процесс расчета стоимости установки.
ms.assetid: be9a8382-c892-44ae-8b59-c665b5cca2d2
title: Действие Костинитиализе
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 251bb0ae7508c87cd0af7ab81196c5d739e923a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127142170"
---
# <a name="costinitialize-action"></a>Действие Костинитиализе

Действие Костинитиализе инициирует процесс [*расчета стоимости*](c-gly.md) установки.

## <a name="sequence-restrictions"></a>Ограничения последовательности

Любые стандартные или [Настраиваемые](custom-actions.md) действия, влияющие на стоимость, должны быть упорядочены перед действием костинитиализе. Вызовите действие [филекост](filecost-action.md) сразу после действия костинитиализе. Затем вызовите действие [костфинализе](costfinalize-action.md) , следующее за действием костинитиализе, чтобы сделать все окончательные вычисления затрат доступными для установщика через таблицу [Component](component-table.md) .

## <a name="actiondata-messages"></a>Сообщения Актиондата

Нет сообщений Актиондата.

## <a name="remarks"></a>Remarks

Действие Костинитиализе загружает таблицу компонентов и таблицу [компонентов](feature-table.md) в память.

Дополнительные сведения об обработке [*затрат*](c-gly.md) в установщике см. в разделе [стоимость файлов](file-costing.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Стоимость файлов](file-costing.md)
</dt> </dl>

 

 



