---
title: Логическое значение (WMI)
description: '\_Параметр VT bool, принимающий значение Variant \_ TRUE (&\# 8211; 1) или вариант \_ false (0).'
ms.assetid: 3928ff39-ed17-4a61-bb72-a3c9be16ae45
ms.tgt_platform: multiple
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 569f7ce633bfb70fdba5e7055a80ad73ebd0fb6c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066527"
---
# <a name="boolean-wmi"></a>Логическое значение (WMI)

Логический тип данных — это \_ параметр логического типа VT, принимающий значение Variant \_ true (– 1) или Variant \_ false (0). В следующей таблице приведена разница между программными представлениями логического значения **true** в C/C++ и типом автоматизации.

| Язык   | Значение         | Числовое значение |
|------------|---------------|-----------------|
| C/C++      | **TRUE**      | 1               |
| Служба автоматизации | ВАРИАНТ \_ true | –1              |

Оба типа являются ненулевыми и, следовательно, не равны **false**, но имеют разные представления для **true**.
