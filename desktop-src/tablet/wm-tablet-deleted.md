---
description: Сообщение об удалении планшета WM отправляется \_ \_ при удалении устройства планшета из Windows.
ms.assetid: af5be7f0-a213-49a1-800e-c922281522c8
title: Сообщение WM_TABLET_DELETED (Тпкшрд. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: da8ade03d199f8ee7a258b9db2aeea039fd725e4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362889"
---
# <a name="wm_tablet_deleted-message"></a>\_ \_ Сообщение об удалении ПЛАНШЕТа WM

Сообщение **об \_ \_ удалении** планшета WM отправляется при удалении устройства планшета из Windows.


```C++
#define WM_TABLET_DEFBASE   0x02C0
#define WM_TABLET_DELETED   (WM_TABLET_DEFBASE + 9)     
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс удаляемого устройства планшета.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Это сообщение отправляется всем окнам верхнего уровня в системе, включая отключенные или невидимые ненадлежащие окна, перекрывающиеся окна и всплывающие окна; но сообщение не отправляется в дочерние окна.

Индексы, переданные в параметре *wParam* , связаны с индексом, используемым методом [**Итаблетманажер:: DataTable**](/previous-versions/windows/desktop/legacy/aa373683(v=vs.85)) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                        |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                            |
| Заголовок<br/>                   | <dl> <dt>Тпкшрд. h</dt> </dl> |



 

 
