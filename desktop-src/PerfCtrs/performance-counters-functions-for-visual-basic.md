---
description: Для работы с данными производительности в Visual Basic можно использовать следующие функции.
ms.assetid: c78eeb43-c713-42cc-a38f-f8aaa04f8dae
title: Функции счетчиков производительности для Visual Basic
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c68fa9b417f6db987110d03fc0c3c88a920adf8cd70cf0ff5f844f26c0ef5c35
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120033524"
---
# <a name="performance-counters-functions-for-visual-basic"></a>Функции счетчиков производительности для Visual Basic

> [!IMPORTANT]
> Функции, описанные в этом разделе, могут быть изменены или недоступны в будущем. Вместо этого корпорация Майкрософт рекомендует использовать функции, описанные в разделе [функции счетчиков производительности](performance-counters-functions.md).

Для работы с данными производительности в Visual Basic можно использовать следующие функции.

- [**пдхклосекуери**](/windows/desktop/api/Pdh/nf-pdh-pdhclosequery)
- [**пдхколлекткуеридата**](/windows/desktop/api/Pdh/nf-pdh-pdhcollectquerydata)
- [**пдхремовекаунтер**](/windows/desktop/api/Pdh/nf-pdh-pdhremovecounter)
- [**пдхвбаддкаунтер**](pdhvbaddcounter.md)
- [**пдхвбкреатекаунтерпаслист**](pdhvbcreatecounterpathlist.md)
- [**пдхвбжеткаунтерпаселементс**](pdhvbgetcounterpathelements.md)
- [**пдхвбжеткаунтерпасфромлист**](pdhvbgetcounterpathfromlist.md)
- [**пдхвбжетдаублекаунтервалуе**](pdhvbgetdoublecountervalue.md)
- [**пдхвбжетлогфилесизе**](pdhvbgetlogfilesize.md)
- [**пдхвбжетонекаунтерпас**](pdhvbgetonecounterpath.md)
- [**пдхвбисгудстатус**](pdhvbisgoodstatus.md)
- [**пдхвбопенлог**](pdhvbopenlog.md)
- [**пдхвбопенкуери**](pdhvbopenquery.md)
- [**пдхвбупдателог**](pdhvbupdatelog.md)

> [!NOTE]
> `PdhVb***`Функции работают с сеансом на уровне процесса и не являются потокобезопасными. Эти функции следует использовать только из простых однопотоковых приложений.
