---
description: ICE84 проверяет таблицу Адвтексекутесекуенце, таблицу Админексекутесекуенце и таблицу Инсталлексекутесекуенце, чтобы убедиться, что следующие стандартные действия не были заданы с условиями в поле Condition.
ms.assetid: 0d1bbf4b-ffab-409e-a292-891dfa823433
title: ICE84
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2af31c343db973481bd69599fadc9c632bbc6dc58a473a69015b3eb0fbe781d5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119895004"
---
# <a name="ice84"></a>ICE84

ICE84 проверяет таблицу [адвтексекутесекуенце](advtexecutesequence-table.md), [таблицу Админексекутесекуенце](adminexecutesequence-table.md)и таблицу [инсталлексекутесекуенце](installexecutesequence-table.md) , чтобы убедиться, что следующие [стандартные действия](standard-actions.md) не были заданы с условиями в поле Condition.

-   [Действие Костинитиализе](costinitialize-action.md)
-   [Действие Костфинализе](costfinalize-action.md)
-   [Действие Филекост](filecost-action.md)
-   [Действие Инсталлвалидате](installvalidate-action.md)
-   [Действие Инсталлинитиализе](installinitialize-action.md)
-   [Действие функции InstallFinalize](installfinalize-action.md)
-   [Действие Процесскомпонентс](processcomponents-action.md)
-   [Действие Публишфеатурес](publishfeatures-action.md)
-   [Действие Публишпродукт](publishproduct-action.md)
-   [Действие Регистерпродукт](registerproduct-action.md)
-   [Действие Унпублишфеатурес](unpublishfeatures-action.md)

При обнаружении условий ICE84 отправляет предупреждение.

## <a name="result"></a>Результат

ICE84 отправляет следующее предупреждение.



| ICE84, ошибка                                                             | Описание                                           |
|-------------------------------------------------------------------------|-------------------------------------------------------|
| Действие " \[ 1 \] ", найденное в таблице% s, является обязательным действием с условием. | Было создано обязательное действие с условием. |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по ICE](ice-reference.md)
</dt> </dl>

 

 



