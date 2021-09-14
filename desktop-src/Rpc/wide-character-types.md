---
title: Типы Wide-Character
description: Microsoft RPC поддерживает широкий тип символов WCHAR \_ t.
ms.assetid: 1a601461-df34-456d-93e8-4cf0b655cf2c
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 821d69999a0ec7e175409120f223721defd6cd10
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146733"
---
# <a name="wide-character-types"></a>Типы Wide-Character

Microsoft RPC поддерживает широкий тип символов [**WCHAR \_ t**](/windows/desktop/Midl/wchar-t). Тип расширенных символов использует 2 байта для каждого символа. Определение языка ANSI C позволяет инициализировать длинные и длинные строки следующим образом:

``` syntax
wchar_t wcInitial = L'a';
wchar_t * pwszString = L"Hello, world";
```

 

 