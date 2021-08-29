---
description: Определяет, какие сертификаты в цепочке сохраняются.
ms.assetid: 6f9e28e6-b01f-4803-8259-8ab73abeecf8
title: Перечисление CAPICOM_CERTIFICATE_INCLUDE_OPTION (CAPICOM. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAPICOM_CERTIFICATE_INCLUDE_OPTION
api_type:
- HeaderDef
api_location:
- Capicom.h
ms.openlocfilehash: 5b6bb2cd36d6ce8ca422d680a05a1e84318d745981a8ca15d9de0be3dfe45c03
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119879394"
---
# <a name="capicom_certificate_include_option-enumeration"></a>\_ \_ Перечисление параметров для включения CAPICOM Certificate \_

Тип **перечисления \_ "CAPICOM Certificate \_ include \_ "** определяет, какие сертификаты в цепочке сохраняются. Этот тип перечисления появился в CAPICOM 2,0.

## <a name="members"></a>Элементы



| Член                                                 | Описание                                                                           | Значение |
|--------------------------------------------------------|---------------------------------------------------------------------------------------|-------|
| **CAPICOM \_ Certificate \_ включает \_ цепочку, \_ кроме \_ root** | Сохраняет все сертификаты в цепочке, за исключением корневой сущности.<br/> | 0     |
| **CAPICOM \_ Certificate \_ включает \_ всю \_ цепочку**        | Сохраняет всю цепочку сертификатов.<br/>                                      | 1     |
| **CAPICOM \_ Certificate \_ — \_ только конечная \_ сущность \_**   | Сохраняет только сертификат конечного объекта.<br/>                                     | 2     |



## <a name="remarks"></a>Remarks

Тип **перечисления \_ \_ \_ "CAPICOM Certificate include** " используется методом [**Certificate. Save**](certificate-save.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------------|--------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                |
| Заголовок<br/>          | <dl> <dt>CAPICOM. h</dt> </dl> |



 

 




