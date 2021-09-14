---
description: Свойство Context Возвращает контекст этого продукта.
ms.assetid: aa772a95-eb4e-45af-9788-9833d62139e8
title: Свойство Product. Context
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Product.Context
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 8334ca57d552681afeb77d0b213eca8b92bc1234
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246430"
---
# <a name="productcontext-property"></a>Свойство Product. Context

Свойство **context** Возвращает контекст этого продукта.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Product.Context
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Это свойство может возвращать одно из следующих значений.



| Контекст                        | Значение | Значение                           |
|--------------------------------|-------|-----------------------------------|
| МСИИНСТАЛЛКОНТЕКСТ \_ усерманажед | 1     | Продукты в управляемом контексте.   |
| \_пользователь мсиинсталлконтекст        | 2     | Продукты в неуправляемом контексте. |
| МСИИНСТАЛЛКОНТЕКСТ \_ компьютер     | 4     | Продукты в контексте компьютера.   |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик 3,0 или более поздней версии на Windows Server 2003, Windows XP и Windows 2000<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                                                   |
| IID<br/>     | IID \_ ипродукт определен как 000C10A0-0000-0000-C000-000000000046<br/>                                                                                                                                                                                                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Продукта**](product-object.md)
</dt> <dt>

[не поддерживается в установщик Windows 2,0 и более ранних версиях](not-supported-in-windows-installer-version-2-0.md)
</dt> </dl>

 

 




