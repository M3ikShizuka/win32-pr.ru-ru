---
description: Сообщение, \_ добавленное планшетом WM, отправляется \_ при добавлении планшетного устройства в Windows.
ms.assetid: 74323b34-2364-47eb-b8ac-b97546e43b32
title: Сообщение WM_TABLET_ADDED (Тпкшрд. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a9c56b475eb63c292d2638d5a34b831862da967868944f823c90b184bdbc076a
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119934334"
---
# <a name="wm_tablet_added-message"></a>\_Сообщение, \_ добавленное ПЛАНШЕТом WM

Сообщение **, \_ \_ добавленное планшетом WM** , отправляется при добавлении планшетного устройства в Windows.


```C++
#define WM_TABLET_DEFBASE  0x02C0
#define WM_TABLET_ADDED    (WM_TABLET_DEFBASE + 8)      
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс добавляемого устройства планшета

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется.

</dd> </dl>

## <a name="remarks"></a>Remarks

Это сообщение отправляется всем окнам верхнего уровня в системе, включая отключенные или невидимые ненадлежащие окна, перекрывающиеся окна и всплывающие окна; но сообщение не отправляется в дочерние окна.

Индексы, переданные в параметре *wParam* , связаны с индексом, используемым методом [**Итаблетманажер:: DataTable**](/previous-versions/windows/desktop/legacy/aa373683(v=vs.85)) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                        |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                            |
| Заголовок<br/>                   | <dl> <dt>Тпкшрд. h</dt> </dl> |



 

 
