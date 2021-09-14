---
title: Сообщение CCM_GETVERSION (Коммктрл. h)
description: Возвращает номер версии элемента управления, заданного последним \_ сообщением CCM сетверсион.
ms.assetid: c4b401d7-bba0-430c-b368-c363d49b3411
keywords:
- элементы управления Windows сообщений CCM_GETVERSION
topic_type:
- apiref
api_name:
- CCM_GETVERSION
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5bd302774f8821b51a4abaf72bccc403e7302e6e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127145250"
---
# <a name="ccm_getversion-message"></a>Сообщение CCM для \_ версии

Возвращает номер версии элемента управления, заданного последним сообщением [**CCM \_ сетверсион**](ccm-setversion.md) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает номер версии, заданный последним сообщением [**CCM \_ сетверсион**](ccm-setversion.md) . Если такое сообщение не было отправлено, оно возвращает ноль.

## <a name="remarks"></a>Remarks

Это сообщение не возвращает версию библиотеки DLL. Сведения об использовании [**дллжетверсион**](/windows/desktop/api/shlwapi/nc-shlwapi-dllgetversionproc) для получения текущей версии DLL см. в статье [версии оболочки](common-control-versions.md) .

> [!Note]  
> Номер версии задается для каждого элемента управления и может отличаться для всех элементов управления.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

