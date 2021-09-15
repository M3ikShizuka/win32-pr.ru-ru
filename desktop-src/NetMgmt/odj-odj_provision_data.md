---
title: ODJ_PROVISION_DATA
description: Определение ODJ_PROVISION_DATA IDL
ms.assetid: ff623d04-ad3f-4846-b9de-aaa280713018
ms.topic: reference
ms.date: 10/12/2020
ms.reviewer: jsimmons
ms.openlocfilehash: f07d8c200103fa21afc080c60157645fe6730766
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566943"
---
# <a name="odj_provision_data-structure"></a>Структура ODJ_PROVISION_DATA

Задает внешнюю структуру сериализации, используемую API-интерфейсами автономного присоединение к домену.

## <a name="syntax"></a>Синтаксис

```C++
typedef struct _ODJ_PROVISION_DATA
{
    ULONG ulVersion;
    ULONG ulcBlobs;
    [size_is(ulcBlobs)] PODJ_BLOB pBlobs;
} ODJ_PROVISION_DATA;
```

## <a name="members"></a>Участники

### <a name="ulversion"></a>улверсион

Это значение должно быть равно 1.

### <a name="ulcblobs"></a>улкблобс

Это значение должно быть равно количеству элементов в массиве Пблобс.

### <a name="pblobs"></a>пблобс

Указывает на массив структур ODJ_BLOB.

## <a name="see-also"></a>См. также раздел

[**Определения IDL для автономного присоединение к домену**](odj-idl.md)

[**\_большой двоичный объект ODJ**](odj-odj_blob.md)


