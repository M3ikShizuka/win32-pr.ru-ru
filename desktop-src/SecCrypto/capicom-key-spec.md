---
description: Перечисление ключевых спецификаций CAPICOM \_ \_ определяет ключевые спецификации.
ms.assetid: e4aaaf69-ab28-4e8c-8a8a-6dc662299865
title: Перечисление CAPICOM_KEY_SPEC (CAPICOM. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAPICOM_KEY_SPEC
api_type:
- HeaderDef
api_location:
- Capicom.h
ms.openlocfilehash: 153f0431d78ff595b4d568fd7a677abea0d28be7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171147"
---
# <a name="capicom_key_spec-enumeration"></a>\_ \_ Перечисление СПЕЦИФИКАЦИй CAPICOM

Перечисление **\_ ключевых \_** спецификаций CAPICOM определяет ключевые спецификации.

## <a name="members"></a>Элементы



| Член                              | Описание                                                | Значение |
|-------------------------------------|------------------------------------------------------------|-------|
| **\_ \_ КЭЙЕКСЧАНЖЕ спецификация CAPICOM \_** | Ключ можно использовать для шифрования и подписывания.<br/> | 1     |
| **\_ \_ подпись спецификации CAPICOM \_**   | Ключ можно использовать только для подписывания.<br/>           | 2     |



## <a name="remarks"></a>Комментарии

Перечисление **\_ ключевых \_ спецификаций CAPICOM** используется следующими методами и свойствами:

-   [**PrivateKey. keySpec**](privatekey-keyspec.md) , свойство.
-   Метод [**PrivateKey. Open**](privatekey-open.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|--------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                |
| Заголовок<br/>          | <dl> <dt>CAPICOM. h</dt> </dl> |



 

 




