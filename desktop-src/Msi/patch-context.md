---
description: Свойство Context Возвращает контекст этого исправления.
ms.assetid: 09c92b0b-44f3-4355-8171-03da8ba32757
title: Свойство patch. Context
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Patch.Context
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 3316c71c5de15a777ce7e4559b7ee52e9efcb61200bd72b8898440e56bb4f392
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120042424"
---
# <a name="patchcontext-property"></a>Свойство patch. Context

Свойство **context** Возвращает контекст этого исправления.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Patch.Context
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Это свойство возвращает одно из следующих значений.



| Контекст                        | Значение | Значение                        |
|--------------------------------|-------|--------------------------------|
| МСИИНСТАЛЛКОНТЕКСТ \_ усерманажед | 1     | Исправление в управляемом контексте.   |
| \_пользователь мсиинсталлконтекст        | 2     | Исправление в неуправляемом контексте. |
| МСИИНСТАЛЛКОНТЕКСТ \_ компьютер     | 4     | Исправление в контексте компьютера.   |



 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик 3,0 или более поздней версии на Windows Server 2003, Windows XP и Windows 2000<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                                                   |
| IID<br/>     | IID \_ ипатч определен как 000C10A1-0000-0000-C000-000000000046<br/>                                                                                                                                                                                                            |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Patch**](patch-object.md)
</dt> <dt>

[не поддерживается в установщик Windows 2,0 и более ранних версиях](not-supported-in-windows-installer-version-2-0.md)
</dt> </dl>

 

 




