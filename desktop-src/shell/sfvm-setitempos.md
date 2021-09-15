---
description: Задает позицию элемента в представлении оболочки. Используется \_ сообщением шшеллфолдервиев.
title: Сообщение SFVM_SETITEMPOS (Шлобж. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: b89f2d62-095b-4cad-a47e-2d41e122cb3e
api_name:
- SFVM_SETITEMPOS
api_type:
- HeaderDef
api_location:
- Shlobj.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 450aeabee6e5edeba466e4a5fe64725c13eea32b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460360"
---
# <a name="sfvm_setitempos-message"></a>\_Сообщение сфвм сетитемпос

Задает позицию элемента в представлении оболочки. Используется [**\_ сообщением шшеллфолдервиев**](/windows/desktop/api/shlobj_core/nf-shlobj_core-shshellfolderview_message).


```C++

                SFVM_SETITEMPOS 

    lParam = (LPSFV_SETITEMPOS)&sip;

            
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*модуль SIP* \[ окне\]
</dt> <dd>

Указатель на структуру [**\_ сетитемпос СФВ**](/windows/desktop/api/Shlobj/ns-shlobj-sfv_setitempos) .

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 1 (SP1), \[ только классические приложения\]<br/>                                |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Шлобж. h</dt> </dl> |



 

 




