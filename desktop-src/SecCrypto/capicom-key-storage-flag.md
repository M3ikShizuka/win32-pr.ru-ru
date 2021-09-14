---
description: '\_ \_ \_ Перечисление флагов хранилища CAPICOM определяет флаги хранилища ключей.'
ms.assetid: 326cef75-24a5-4dc9-a7e9-a63dd3d8de54
title: Перечисление CAPICOM_KEY_STORAGE_FLAG (CAPICOM. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAPICOM_KEY_STORAGE_FLAG
api_type:
- HeaderDef
api_location:
- Capicom.h
ms.openlocfilehash: 9edbc3a5ac3396e528ebbb5390c4b07c24770e58
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171143"
---
# <a name="capicom_key_storage_flag-enumeration"></a>\_ \_ \_ Перечисление ФЛАГов хранилища CAPICOM

Перечисление **\_ \_ \_ флагов хранилища CAPICOM** определяет флаги хранилища ключей.

## <a name="members"></a>Элементы



| Член                                     | Описание                           | Значение |
|--------------------------------------------|---------------------------------------|-------|
| **\_хранилище CAPICOM \_ key \_ по умолчанию**         | Хранилище ключей по умолчанию.<br/>       | 0     |
| **\_хранилище CAPICOM Key, \_ \_ экспортируемое**      | Ключ доступен для экспорта.<br/>     | 1     |
| **\_ \_ \_ защищенное пользователем хранилище CAPICOM key \_** | Ключ защищен пользователем.<br/> | 2     |



## <a name="remarks"></a>Комментарии

Это перечисление используется следующим методом:

-   [**Certificate. Load**](certificate-load.md)
-   [**Store. Load**](store-load.md)

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|--------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                |
| Заголовок<br/>          | <dl> <dt>CAPICOM. h</dt> </dl> |



 

 




