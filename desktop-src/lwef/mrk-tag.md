---
title: Тег МРК
description: Тег МРК
ms.assetid: 1bc04853-f919-4f6f-90c2-21ac836bb1e4
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 805a66b9ce5863bda7b7b95317bcab9cf1d80f32
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168263"
---
# <a name="mrk-tag"></a>Тег МРК

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Определяет закладку в речевом тексте.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

**\\ МРК =**_число_*_\\_*



| Часть     | Описание                                        |
|----------|----------------------------------------------------|
| *number* | Длинное целочисленное значение, идентифицирующее закладку. |



 

</dd> </dl>

### <a name="remarks"></a>Remarks

Когда сервер обрабатывает закладку, он создает событие закладки. Необходимо указать число больше нуля (0) и не равно 2147483647 или 2147483646.

 

 




