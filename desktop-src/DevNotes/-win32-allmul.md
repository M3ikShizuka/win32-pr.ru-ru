---
title: _allmul подпрограммы
description: Умножает два целых числа ЛОНГЛОНГ или УЛОНГЛОНГ.
ms.assetid: na
ms.topic: reference
ms.date: 04/29/2019
ms.keywords: _allmul, ntoskrnl.exe!_allmul
topic_type:
- APIRef
api_type:
- DllExport
api_location:
- ntoskrnl.exe
api_name:
- _allmul
targetos: Windows
ms.openlocfilehash: 38795bf755574ecf1a21ddcdb3655b14a4751a51fc6eca61118734f42e0bc3e2
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119386864"
---
# <a name="_allmul-routine"></a>\_подпрограммы аллмул

Умножает два целых числа **лонглонг** или **улонглонг** .
Например, чтобы умножить два значения Int64, компилятор может создать вызов подпрограммы **\_ аллмул** .

## <a name="remarks"></a>Remarks

Подпрограммы **\_ аллмул** — это вспомогательная подпрограммы для компилятора C.
Будет ли компилятор использовать **\_ аллмул** , полностью зависит от набора оптимизации.

Эта подпрограммы используется только на платформах x86.
