---
description: Система передает \_ событие ДБТ девнодес \_ Changed Device, когда устройство было добавлено или удалено из системы. Приложения, поддерживающие списки устройств в системе, должны обновлять свои списки.
ms.assetid: 62acc633-7dad-4792-a5a2-1f95356479d1
title: Событие DBT_DEVNODES_CHANGED (ДБТ. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1450e9a87d541e5df3d9a9286e48601697e6aaae
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127164447"
---
# <a name="dbt_devnodes_changed-event"></a>\_ \_ Событие изменения ДБТ девнодес

Система передает \_ событие ДБТ девнодес \_ Changed Device, когда устройство было добавлено или удалено из системы. Приложения, поддерживающие списки устройств в системе, должны обновлять свои списки.

Чтобы транслировать это событие устройства, система использует сообщение [**WM \_ девицечанже**](wm-devicechange.md) с параметром *wParam* , установленным в ДБТ \_ Девнодес \_ Changed, и параметр *lParam* имеет значение 0.


```C++
LRESULT CALLBACK WindowProc(
  HWND hwnd,       // handle to window
  UINT uMsg,       // WM_DEVICECHANGE
  WPARAM wParam,   // device-change event
  LPARAM lParam    // event-specific data
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*HWND* 
</dt> <dd>

Дескриптор окна.

</dd> <dt>

*Uiacp* 
</dt> <dd>

Идентификатор сообщения [**WM \_ девицечанже**](wm-devicechange.md) .

</dd> <dt>

*wParam* 
</dt> <dd>

Задайте значение ДБТ \_ девнодес \_ изменено.

</dd> <dt>

*lParam* 
</dt> <dd>

Задайте нулевое значение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true**.

## <a name="remarks"></a>Комментарии

Дополнительные сведения о том, какое устройство было добавлено или удалено из системы, не существует. Приложения, для которых требуется дополнительная информация, должны регистрироваться для уведомления устройства с помощью функции [**регистердевиценотификатион**](/windows/desktop/api/Winuser/nf-winuser-registerdevicenotificationa) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2003<br/>                                                   |
| Заголовок<br/>                   | <dl> <dt>ДБТ. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[События устройства](device-events.md)
</dt> <dt>

[События управления устройствами](device-management-events.md)
</dt> <dt>

[**расвещание для разработки в \_ \_ HDR**](/windows/desktop/api/Dbt/ns-dbt-dev_broadcast_hdr)
</dt> <dt>

[**WM \_ девицечанже**](wm-devicechange.md)
</dt> </dl>

 

 




