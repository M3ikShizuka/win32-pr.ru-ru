---
description: ICE77 проверяет, что настраиваемые действия с набором Мсидбкустомактионтипеинскрипт bit упорядочены после действия Инсталлинитиализе и перед действием функции InstallFinalize.
ms.assetid: 291cf731-b7e6-44c2-a8ec-78e0e037d1f5
title: ICE77
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5910b814a9cee6da87a76594949f2ad3250bbdd55c3666d0f500ea3a64ae3730
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119894984"
---
# <a name="ice77"></a>ICE77

ICE77 проверяет, что настраиваемые действия с набором **мсидбкустомактионтипеинскрипт** bit упорядочены после [действия инсталлинитиализе](installinitialize-action.md) и перед [действием функции InstallFinalize](installfinalize-action.md). ICE77 проверяет последовательность в [таблице инсталлексекутесекуенце](installexecutesequence-table.md) и [таблице админексекутесекуенце](adminexecutesequence-table.md).

## <a name="result"></a>Результат

ICE77 отправляет ошибку, если настраиваемое действие в скрипте выполняется последовательно перед действием Инсталлинитиализе или после действия функции InstallFinalize.

ICE77 отправляет сообщение об ошибке, если отсутствует действие Инсталлинитиализе или функции InstallFinalize.

## <a name="example"></a>Пример

ICE77 сообщает о следующих ошибках в примере:

``` syntax
InstallFinalize is missing from 'InstallExecuteSequence'. 
CA_InScriptInstall is a in-script custom action. It must be sequenced 
before the InstallFinalize action.
 
CA_InScriptAdmin is a in-script custom action.  It must be sequenced 
in between the InstallInitialize action and the InstallFinalize action 
in the AdminExecuteSequence Sequence table.
```

[Таблица CustomAction](customaction-table.md) (частичная)



| Действие              | Тип |
|---------------------|------|
| \_ИНСКРИПТИНСТАЛЛ CA | 1025 |
| \_ИНСКРИПТАДМИН CA   | 1026 |



 

[Таблица инсталлексекутесекуенце](installexecutesequence-table.md) (частичная)



| Действие              | Последовательность |
|---------------------|----------|
| \_ИНСКРИПТИНСТАЛЛ CA | 2000     |
| инсталлинитиализе   | 1500     |



 

[Таблица админексекутесекуенце](adminexecutesequence-table.md) (частичная)



| Действие            | Последовательность |
|-------------------|----------|
| \_ИНСКРИПТАДМИН CA | 1400     |
| инсталлинитиализе | 1500     |
| Функции InstallFinalize   | 6600     |



 

Чтобы устранить ошибки, поочередно заполните пользовательские действия в скрипте после действия Инсталлинитиализе и перед действием функции InstallFinalize. Действия Инсталлинитиализе и функции InstallFinalize должны присутствовать в таблице Инсталлексекутесекуенце и таблице Админексекутесекуенце.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по ICE](ice-reference.md)
</dt> </dl>

 

 



