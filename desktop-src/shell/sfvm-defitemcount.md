---
description: 'Позволяет объекту обратного вызова указывать количество элементов в представлении папки. Используется Ишеллфолдервиевкб:: Мессажесфвкб.'
title: Сообщение SFVM_DEFITEMCOUNT (Шлобж. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: 62306eaa-e52e-432b-9233-d990519d5739
api_name:
- SFVM_DEFITEMCOUNT
api_type:
- HeaderDef
api_location:
- Shlobj.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 29e92aca1a1f52c0722c890f097ddab33255e814ec35768208644a3a9d814353
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119709884"
---
# <a name="sfvm_defitemcount-message"></a>\_Сообщение сфвм дефитемкаунт

Позволяет объекту обратного вызова указывать количество элементов в представлении папки. Используется [**ишеллфолдервиевкб:: мессажесфвкб**](/windows/win32/api/shlobj_core/nf-shlobj_core-ishellfolderviewcb-messagesfvcb).


```C++
SFVM_DEFITEMCOUNT 

    lParam = (LPARAM)(UINT*) cItems;

            
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Цитемс* \[ заполняет\]
</dt> <dd>

Число элементов в представлении папки.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Шлобж. h</dt> </dl> |



 

 
