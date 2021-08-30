---
description: ICEM03 проверяет, что все действия в модуле являются базовыми действиями или являются производными от действительного базового действия.
ms.assetid: 8e2b5921-32cf-45e8-9906-30002574a712
title: ICEM03
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7f061fbf63fa1874fef8764aee56b3e7caa41976a8280802041c54f088c663c7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119894614"
---
# <a name="icem03"></a>ICEM03

ICEM03 проверяет, что все действия в модуле являются базовыми действиями или являются производными от действительного базового действия.

Модуль слияния ICEs хранится в файле слияния Module. CUB, который называется Мержемод. CUB, а не в файле. CUB, содержащем значение ICEs, используемое для проверки пакета.

## <a name="result"></a>Результат

ICEM03 отправляет сообщения об ошибках для модуля, содержащего действия в таблице последовательности, которые не являются базовым действием или являются производными от действительного базового действия.

## <a name="example"></a>Пример

ICEM03 отправляет следующие сообщения об ошибках для модуля, содержащего записи базы данных, показанные ниже.

``` syntax
The action 'Action1' in the 'ModuleInstallExecuteSequence' table is 
orphaned. It is not a valid base action and does not derive from a 
valid base action.
The action 'Action2' in the 'ModuleInstallExecuteSequence' table is 
orphaned. It is not a valid base action and does not derive from a 
valid base action.
```

[Таблица Модулеинсталлексекутесекуенце](moduleinstallexecutesequence-table.md)



| Действие  | Последовательность | басеактион | После | Условие |
|---------|----------|------------|-------|-----------|
| Action1 превышают |          | Action2    | 0     |           |
| Action2 |          | Action1 превышают    | 0     |           |



 

ICEM03 отправляет ошибки для этих двух действий, так как они ссылаются друг на друга как на базовые действия в таблице Модулеинсталлексекутесекуенце. Все действия в таблицах [модулеадминуисекуенце](moduleadminuisequence-table.md), [модулеадминексекутесекуенце](moduleadminexecutesequence-table.md), [модулеадвтуисекуенце](moduleadvtuisequence-table.md), [модулеадвтексекутесекуенце](moduleadvtexecutesequence-table.md), [ModuleInstallUISequence](moduleinstalluisequence-table.md)и [ModuleInstallExecuteSequence](moduleinstallexecutesequence-table.md) должны быть базовыми или производными от сочетания другого действия и флага Before и After.

Чтобы устранить эту ошибку, определите базовые действия для двух действий. Добавьте запись для базовых действий с порядковым номером по умолчанию. Для Action1 превышают и Action2 введите имена базовых действий в столбце Басеактион и 0 или 1 в столбце After.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Ссылка на модуль слияния ICE](merge-module-ice-reference.md)
</dt> </dl>

 

 



