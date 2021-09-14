---
description: Сбор метрик секции
ms.assetid: 2dc35011-24fa-49df-9cf8-96db2de39efa
title: Сбор метрик секции
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6467dfb9c891e7ae57505c8ec3815bfa99e49d8a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066469"
---
# <a name="collecting-partition-metrics"></a>Сбор метрик секции

В некоторых случаях Организация может захотеть собираются сведения об использовании приложения COM+ в целях мониторинга, планирования загрузки и учета ресурсов.

Например, поставщику службы приложений (ASP) может потребоваться начисление клиента на использование ресурсов. Для этого COM+ позволяет получать сведения о событиях и метриках на основе каждого раздела.

Чтобы получить эти сведения для определенной секции, необходимо указать для каждого интерфейса инструментария COM+ элемент идентификатора секции в стандартной структуре событий. Структура событий является первым значением интерфейса инструментария COM+. Дополнительные сведения см. в разделе [интерфейсы инструментария com+](com--instrumentation-interfaces.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Настройка кэша секций](configuring-the-partition-cache.md)
</dt> <dt>

[Группирование приложений в секции](grouping-applications-into-partitions.md)
</dt> <dt>

[Управление локальными секциями](managing-local-partitions.md)
</dt> <dt>

[Управление секциями в Active Directory](managing-partitions-within-active-directory.md)
</dt> <dt>

[Установка прав администратора для секции](setting-administrative-rights-for-a-partition.md)
</dt> </dl>

 

 



