---
description: 'Уведомляет объект обратного вызова о том, что произошло событие, которое влияет на один из его элементов. Используется Ишеллфолдервиевкб:: Мессажесфвкб.'
title: Сообщение SFVM_FSNOTIFY (Шлобж. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: ff159c35-afdf-4147-8dd6-7febd9519b18
api_name:
- SFVM_FSNOTIFY
api_type:
- HeaderDef
api_location:
- Shlobj.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 74c17f9d4b8c8c1979fa7da2d6f0ff63dff74a9b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459427"
---
# <a name="sfvm_fsnotify-message"></a>\_Сообщение сфвм фснотифи

Уведомляет объект обратного вызова о том, что произошло событие, которое влияет на один из его элементов. Используется [**ишеллфолдервиевкб:: мессажесфвкб**](/windows/win32/api/shlobj_core/nf-shlobj_core-ishellfolderviewcb-messagesfvcb).


```C++
SFVM_FSNOTIFY 

    wParam = (WPARAM)(LPCITEMIDLIST*) ppidl;

    lParam = (LPARAM)(DWORD) lEvent;

            
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппидл* \[ окне\]
</dt> <dd>

Указатель ПИДЛ затронутого элемента.

</dd> <dt>

*Левент* \[ окне\]
</dt> <dd>

Значение ШКНЕ, указывающее, какое событие произошло. Список возможных значений см. в разделе [**шчанженотифи**](/windows/desktop/api/shlobj_core/nf-shlobj_core-shchangenotify).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Шлобж. h</dt> </dl> |



 

 
