---
description: 'Позволяет обратному вызову изменять \_ значения CFM XXX, переданные в IContextMenu:: куериконтекстмену.'
title: Сообщение DFM_MODIFYQCMFLAGS (Шлобж. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: 2c87e14d-4cf4-425d-a5fe-9dc7530f0e59
api_name:
- DFM_MODIFYQCMFLAGS
api_type:
- HeaderDef
api_location:
- Shlobj.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: ff90cfb0e0297e7d3276f00f314fce865920663a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460511"
---
# <a name="dfm_modifyqcmflags-message"></a>\_Сообщение DFM модификкмфлагс

Позволяет обратному вызову изменять \_ значения CFM XXX, переданные в [**IContextMenu:: куериконтекстмену**](/windows/desktop/api/shobjidl_core/nf-shobjidl_core-icontextmenu-querycontextmenu).


```C++
DFM_MODIFYQCMFLAGS

    lParam = (LPARAM)(UINT) *puNewFlags;

    wParam = (WPARAM)(UINT) uFlags;         

            
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пуневфлагс* \[ окне\]
</dt> <dd>

Указатель на новые значения флагов.

</dd> <dt>

*уфлагс* \[ окне\]
</dt> <dd>

Флаги, указывающие, как можно изменить контекстное меню. Этот параметр использует значения КМФ \_ xxx, описанные в [**IContextMenu:: куериконтекстмену**](/windows/desktop/api/shobjidl_core/nf-shobjidl_core-icontextmenu-querycontextmenu).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>Шлобж. h</dt> </dl> |



 

 




