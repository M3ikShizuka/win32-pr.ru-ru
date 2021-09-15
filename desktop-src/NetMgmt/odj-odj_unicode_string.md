---
title: ODJ_UNICODE_STRING
description: Определение ODJ_UNICODE_STRING IDL
ms.assetid: a7999df0-d961-4fd7-ae5e-65ad79a9c17c
ms.topic: reference
ms.date: 10/12/2020
ms.reviewer: jsimmons
ms.openlocfilehash: f1134d7b95cca6948932bf9d79fe976d6745448a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566934"
---
# <a name="odj_unicode_string-structure"></a>Структура ODJ_UNICODE_STRING

Содержит строку в Юникоде.

## <a name="syntax"></a>Синтаксис

```C++
typedef struct _ODJ_UNICODE_STRING
{
    USHORT Length;
    USHORT MaximumLength;
    [size_is(MaximumLength/2), length_is(Length/2)] PWSTR Buffer;
} ODJ_UNICODE_STRING, *PODJ_UNICODE_STRING;
```

## <a name="members"></a>Участники

### <a name="length"></a>Длина

Необходимо задать значение, равное количеству байтов в буфере, содержащему строку, не включая знак завершения NULL.

### <a name="maximumlength"></a>MaximumLength

Это значение должно быть равно общему количеству байтов в буфере, не включая знак завершения NULL.

### <a name="buffer"></a>Буфер

Должен быть строкой Юникода.

## <a name="see-also"></a>См. также раздел

[**Определения IDL для автономного присоединение к домену**](odj-idl.md)
