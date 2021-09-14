---
description: Событие изменения параметра питания, отправленное с помощью \_ сообщения окна WM поверброадкаст или обратного вызова уведомления хандлерекс для служб.
ms.assetid: 0bcadb85-47c5-48a9-b3f9-f0a1ca60b503
title: Событие PBT_POWERSETTINGCHANGE (WinUser. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e0f38486d2e5cce1cfe541468e548e92353c9837
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055082"
---
# <a name="pbt_powersettingchange-event"></a>\_Событие ПБТ поверсеттингчанже

Событие изменения параметра питания, отправленное с помощью сообщения окна [**WM \_ поверброадкаст**](wm-powerbroadcast.md) или обратного вызова уведомления [**хандлерекс**](/windows/desktop/api/winsvc/nc-winsvc-lphandler_function_ex) для служб.


```C++
LRESULT 
CALLBACK 
WindowProc( HWND hwnd,      // handle to window
            UINT uMsg,      // WM_POWERBROADCAST
            WPARAM wParam,  // PBT_POWERSETTINGCHANGE
            LPARAM lParam); // Pointer to POWERBROADCAST_SETTING
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*HWND* 
</dt> <dd>

Маркер для окна.

</dd> <dt>*uiacp*</dt> <dd> 

| Значение                                                                                                                                                                                                                                                                   | Значение                        |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------|
| <span id="WM_POWERBROADCAST"></span><span id="wm_powerbroadcast"></span><dl> <dt>**[**WM \_ ПОВЕРБРОАДКАСТ**](wm-powerbroadcast.md)**</dt> <dt>536 (0x218)</dt> </dl> | Идентификатор сообщения.<br/> |



 

</dd> <dt>*wParam*</dt> <dd> 

| Значение                                                                                                                                                                                                                                                        | Значение                      |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|
| <span id="PBT_POWERSETTINGCHANGE"></span><span id="pbt_powersettingchange"></span><dl> <dt>**ПБТ \_ ПОВЕРСЕТТИНГЧАНЖЕ**</dt> <dt>32787 (0x8013)</dt> </dl> | Идентификатор события.<br/> |



 

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**\_ параметра поверброадкаст**](/windows/desktop/api/WinUser/ns-winuser-powerbroadcast_setting) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>WinUser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[События управления питанием](power-management-events.md)
</dt> <dt>

[**хандлерекс**](/windows/desktop/api/winsvc/nc-winsvc-lphandler_function_ex)
</dt> <dt>

[**WM \_ поверброадкаст**](wm-powerbroadcast.md)
</dt> <dt>

[**\_параметр поверброадкаст**](/windows/desktop/api/WinUser/ns-winuser-powerbroadcast_setting)
</dt> </dl>

 

