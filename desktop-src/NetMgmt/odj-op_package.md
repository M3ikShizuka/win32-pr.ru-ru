---
title: OP_PACKAGE
description: Определение OP_PACKAGE IDL
ms.assetid: 065266a6-6db5-4113-bd2b-22ac6063236d
ms.topic: reference
ms.date: 10/12/2020
ms.reviewer: jsimmons
ms.openlocfilehash: 81fdc237b731489f7ac501a4e053e62d744b0fdef77c5b630cd478dede5aeda5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119911494"
---
# <a name="op_package-structure"></a>Структура OP_PACKAGE

Содержит структуру, содержащую сериализованные OP_PACKAGE_COLLECTION.

## <a name="syntax"></a>Синтаксис

```C++
typedef struct _OP_PACKAGE
{
    GUID    EncryptionType;
    OP_BLOB EncryptionContext;
    OP_BLOB WrappedPartCollection;
    ULONG   cbDecryptedPartCollection;
    OP_BLOB Extension;
} OP_PACKAGE, *POP_PACKAGE;
```

## <a name="members"></a>Члены

### <a name="encryptiontype"></a>EncryptionType

Зарезервировано для будущего использования и должно быть установлено в значение GUID_NULL.

### <a name="encryptioncontext"></a>енкриптионконтекст

Зарезервировано для будущего использования и должно иметь значение "все нули".

### <a name="wrappedpartcollection"></a>враппедпартколлектион

Структура OP_BLOB, которая содержит сериализованную структуру OP_PACKAGE_COLLECTION.

### <a name="cbdecryptedpartcollection"></a>кбдекриптедпартколлектион

Зарезервировано для будущего использования и должно быть равно нулю.

### <a name="extension"></a>Расширение

Зарезервировано для будущего использования и должно иметь значение "все нули".

## <a name="see-also"></a>См. также раздел

[**Определения IDL для автономного присоединение к домену**](odj-idl.md)

[**\_большой двоичный объект Op**](odj-op_blob.md)

[**\_Коллекция пакетов \_ Op**](odj-op_package_collection.md)
