---
description: Действие Унрегистерфонтс удаляет сведения о регистрации установленных шрифтов из системы.
ms.assetid: 97cbbcbe-eb1c-45f0-91d2-4b17984498ae
title: Действие Унрегистерфонтс
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9fcc847203b72b0e2d92fb5e9a4dc465bebb001b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171576"
---
# <a name="unregisterfonts-action"></a>Действие Унрегистерфонтс

Действие Унрегистерфонтс удаляет сведения о регистрации установленных шрифтов из системы.

## <a name="sequence-restrictions"></a>Ограничения последовательности

Действие [ремовефилес](removefiles-action.md) должно быть вызвано после унрегистерфонтс.

## <a name="actiondata-messages"></a>Сообщения Актиондата



| Поле | Описание данных действия |
|-------|----------------------------|
| \[1\] | Файл шрифта.                 |



 

## <a name="remarks"></a>Комментарии

Действие Унрегистерфонтс выполняется, если файл, указанный в \_ столбце file [таблицы Font](font-table.md) , относится к удаляемому компоненту.

 

 



