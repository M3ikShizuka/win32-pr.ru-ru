---
description: Компоненты указывают типы данных, которые они представляют через тип.
ms.assetid: 19d785d5-09a7-48b9-a0a2-eca3049d67fe
title: Типы компонентов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d1f89355b4b26090b7d43f9753c086b4ccc79df0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461348"
---
# <a name="component-types"></a>Типы компонентов

Компоненты указывают типы данных, которые они представляют через тип.

В настоящее время типы компонентов (см. раздел [**\_ \_ тип компонента VSS**](/windows/desktop/api/VsWriter/ne-vswriter-vss_component_type)) имеют следующие ограничения:

-   Компоненты базы данных
-   Группы файлов

Сведения о реализации типов компонентов см. в разделе [Определение компонентов по модулям записи](definition-of-components-by-writers.md).

Модули записи имеют тип данных, указывающий их использование (см. сведения о [**\_ \_ типе источника VSS**](/windows/desktop/api/VsWriter/ne-vswriter-vss_source_type)). это может быть следующее:

-   транзакционная база данных (например, сервер SQL);
-   Нетранзакционная база данных (например, клиент электронной таблицы)
-   Файловая группа (другая)

Указание типа компонента в качестве базы данных позволяет упростить идентификацию содержимого, позволяет отдельно обрабатывать файлы журналов и данных (Дополнительные сведения см. в разделе [**ивсскреатевритерметадата**](/windows/desktop/api/VsWriter/nl-vswriter-ivsscreatewritermetadata) и [**ивссексаминевритерметадата**](/windows/desktop/api/VsBackup/nl-vsbackup-ivssexaminewritermetadata) ) и обеспечивает более высокий строгий выбор файлов, не разрешая рекурсивного выбора файлов или использования [*альтернативного пути*](vssgloss-a.md) (см. раздел [**ивсскреатевритерметадата:: адддатабасефилес**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-adddatabasefiles) и [**IVssCreateWriterMetadata:: AddDatabaseLogFiles**](/windows/desktop/api/VsWriter/nf-vswriter-ivsscreatewritermetadata-adddatabaselogfiles)).

С другой стороны, с помощью компонента файловой группы, по цене не зная, какие данные он содержит, вы можете получить большую свободу при вставке файлов, так как можно использовать рекурсивную спецификацию и альтернативные пути.

Дополнительные типы компонентов могут быть добавлены в будущем.

 

 



