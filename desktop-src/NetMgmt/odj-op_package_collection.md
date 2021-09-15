---
title: OP_PACKAGE_PART_COLLECTION
description: Определение OP_PACKAGE_PART_COLLECTION IDL
ms.assetid: a7abf011-0335-4869-b4d9-144b2f392241
ms.topic: reference
ms.date: 10/12/2020
ms.reviewer: jsimmons
ms.openlocfilehash: f8eb61397045a382fe5933025a4eeda2f563e838
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566902"
---
# <a name="op_package_part_collection-structure"></a>Структура OP_PACKAGE_PART_COLLECTION

Задает структуру, содержащую массив структур OP_PACKAGE_PART.

## <a name="syntax"></a>Синтаксис

```C++
typedef struct _OP_PACKAGE_PART_COLLECTION
{
    ULONG                                 cParts;
    [size_is(cParts)]   POP_PACKAGE_PART  pParts;
    OP_BLOB                               Extension;
} OP_PACKAGE_PART_COLLECTION, *POP_PACKAGE_PART_COLLECTION;
```

## <a name="members"></a>Участники

### <a name="cparts"></a>кпартс

Содержит количество элементов в Ппартс.

### <a name="pparts"></a>ппартс

Содержит массив структур OP_PACKAGE_PART.

### <a name="extension"></a>Расширение

Зарезервировано для будущего использования и должно иметь значение "все нули".

## <a name="see-also"></a>См. также раздел

[**Определения IDL для автономного присоединение к домену**](odj-idl.md)

[**\_часть пакета \_ Op**](odj-op_package_part.md)

[**\_большой двоичный объект Op**](odj-op_blob.md)

