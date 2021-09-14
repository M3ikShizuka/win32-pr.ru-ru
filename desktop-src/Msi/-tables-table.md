---
description: Таблица Tables \_ является системной таблицей только для чтения, в которой перечислены все таблицы в базе данных. Запросите эту таблицу, чтобы узнать, существует ли таблица.
ms.assetid: d064855b-8c10-476e-9570-cc3ab48ae998
title: Таблица _Tables
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d2dc3ebafd969a07676f64f674f76c3e16ebe059
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127143258"
---
# <a name="_tables-table"></a>\_Таблица таблиц

Таблица Tables \_ является системной таблицей только для чтения, в которой перечислены все таблицы в базе данных. Запросите эту таблицу, чтобы узнать, существует ли таблица.

Таблица Tables \_ содержит следующий столбец.



| Столбец | Type             | Ключ | Допускает значения NULL |
|--------|------------------|-----|----------|
| Имя   | [Text](text.md) | Да   | Нет        |



 

## <a name="column"></a>Столбец

<dl> <dt>

<span id="Name"></span><span id="name"></span><span id="NAME"></span>Безымян
</dt> <dd>

Имя одной из таблиц.

</dd> </dl>

## <a name="remarks"></a>Remarks

поскольку таблица tables \_ является системной таблицей, которую нельзя изменить с помощью запросов SQL, вы не можете получить первичные ключи с помощью функции [**мсидатабасежетпримарикэйс**](/windows/desktop/api/Msiquery/nf-msiquery-msidatabasegetprimarykeysa) или [**свойства примарикэйс**](database-primarykeys.md).

 

 



