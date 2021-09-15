---
description: Что реплицируется
ms.assetid: d1f0bc92-37bc-4de2-876a-e6b8b09da58d
title: Что реплицируется
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: dd2739cb0ff615ddc38f30a7aa9b0a572be5e28a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127457927"
---
# <a name="what-gets-replicated"></a>Что реплицируется

## <a name="applications"></a>Приложения

Все приложения, установленные на исходном компьютере, реплицируются, за исключением следующих:

<dl> <dt>

<span id="Non-COM__application_elements_and_dependencies"></span><span id="non-com__application_elements_and_dependencies"></span><span id="NON-COM__APPLICATION_ELEMENTS_AND_DEPENDENCIES"></span>Не-COM + элементы и зависимости приложений
</dt> <dd>

Администратор несет ответственность за репликацию любого объекта, от которого зависит приложение COM+, но которое неправильно входит в само приложение, например файлы данных и библиотеки DLL. COMREPL не будет реплицировать что-либо за пределы элементов приложения COM+.

</dd> <dt>

<span id="COM__preinstalled_applications"></span><span id="com__preinstalled_applications"></span><span id="COM__PREINSTALLED_APPLICATIONS"></span>Предварительно установленные приложения COM+
</dt> <dd>

Приложения, которые используются внутри COM+ и устанавливаются с помощью программы установки COM+, не реплицируются. Вот некоторые из них.

-   Системное приложение
-   Программы COM+
-   Прослушиватель очереди недоставленных сообщений COM+ QC

</dd> <dt>

<span id="Applications_created_by_IIS"></span><span id="applications_created_by_iis"></span><span id="APPLICATIONS_CREATED_BY_IIS"></span>Приложения, созданные службами IIS
</dt> <dd>

Эти приложения не реплицируются и включают следующее:

-   Внутрипроцессный приложения IIS
-   Служебные программы IIS
-   Все приложения, созданные для изолированных или виртуальных корней в составе пула

</dd> </dl>

## <a name="computer-list"></a>Список компьютеров

Удаленные компьютеры, имена которых находятся в папке **Computers** средства администрирования служб компонентов, не реплицируются с исходного компьютера на целевой компьютер.

## <a name="properties"></a>Свойства

Реплицируются следующие свойства коллекции **локалкомпутер** :

-   TransactionTimeout
-   ресаурцепулинженаблед
-   дкоменаблед
-   дефаултаусентикатионлевел
-   дефаултимперсонатионлевел
-   секурититраккинженаблед
-   Цисенаблед
-   секуререференцесенаблед
-   интернетпортслистед
-   деафулттоинтернетпортс
-   Порты
-   рпкпроксенаблед

Следующие свойства коллекции **локалкомпутер** не реплицируются:

-   Описание
-   аппликатионпроксирсн
-   Маршрутизатор

Описание свойств коллекции **локалкомпутер** см. в разделе [**локалкомпутер**](localcomputer.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Управление файлами](file-management.md)
</dt> <dt>

[Ведение журнала и отчеты об ошибках](logging-and-error-reporting.md)
</dt> <dt>

[Этапы репликации](replication-phases.md)
</dt> <dt>

[Использование COMREPL](using-comrepl.md)
</dt> </dl>

 

 



