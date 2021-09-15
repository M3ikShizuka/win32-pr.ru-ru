---
title: OP_BLOB
description: Определение OP_BLOB IDL
ms.assetid: c215c793-5fad-4baa-97c0-c809040dda1e
ms.topic: reference
ms.date: 10/12/2020
ms.reviewer: jsimmons
ms.openlocfilehash: fab6df11be3bf719f787c40a41a50d948a865474
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566922"
---
# <a name="op_blob-structure"></a>Структура OP_BLOB

Содержит непрозрачный байтовый буфер.

## <a name="syntax"></a>Синтаксис

```C++
typedef struct _OP_BLOB
{
    ULONG                       cbBlob;
    [size_is(cbBlob)]   PBYTE   pBlob;
} OP_BLOB, *POP_BLOB;
```

## <a name="members"></a>Участники

### <a name="cbblob"></a>кбблоб

Задает размер Пблоб в байтах.

### <a name="pblob"></a>пблоб

Указывает на буфер байтов.

## <a name="see-also"></a>См. также раздел

[**Определения IDL для автономного присоединение к домену**](odj-idl.md)
