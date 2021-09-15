---
title: Константы окна проверки нажатия касания
description: Указывает, как сообщения для проверки попадания касания обрабатываются окнами, зарегистрированными с помощью функции Регистертаучхиттестингвиндов.
ms.assetid: CC6CCD0B-882F-4DA7-B886-D4BD18D6060C
topic_type:
- apiref
api_name:
- TOUCH_HIT_TESTING_DEFAULT
- TOUCH_HIT_TESTING_CLIENT
- TOUCH_HIT_TESTING_NONE
api_location:
- winuser.h
api_type:
- HeaderDef
ms.topic: article
ms.date: 02/03/2020
ms.openlocfilehash: 46d577e03eaf918e4f2ea40aae30a2ab5112b630
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569094"
---
# <a name="touch-hit-testing-window-constants"></a>Константы окна проверки нажатия касания

Указывает, как сообщения для проверки попадания касания обрабатываются окнами, зарегистрированными с помощью функции [**регистертаучхиттестингвиндов**](/windows/win32/api/winuser/nf-winuser-registertouchhittestingwindow) .



| Константа/значение                                                                                                                                                                                                                                                   | Описание                                                                                                                            |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| <span id="TOUCH_HIT_TESTING_DEFAULT"></span><span id="touch_hit_testing_default"></span><dl> <dt>**TOUCH_HIT_TESTING_DEFAULT**</dt> <dt>0 (0x0)</dt> </dl> | [**WM_TOUCHHITTESTING**](wm-touchhittesting.md) сообщения не отправляются в целевое окно, но отправляются в дочерние окна.<br/> |
| <span id="TOUCH_HIT_TESTING_CLIENT"></span><span id="touch_hit_testing_client"></span><dl> <dt>**TOUCH_HIT_TESTING_CLIENT**</dt> <dt>1 (0x1)</dt> </dl>    | [**WM_TOUCHHITTESTING**](wm-touchhittesting.md) сообщения отправляются в целевое окно.<br/>                                   |
| <span id="TOUCH_HIT_TESTING_NONE"></span><span id="touch_hit_testing_none"></span><dl> <dt>**TOUCH_HIT_TESTING_NONE**</dt> <dt>2 (0x2)</dt> </dl>          | [**WM_TOUCHHITTESTING**](wm-touchhittesting.md) сообщения не отправляются в целевое окно или дочерние окна.<br/>              |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Winuser. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Константы](constants.md)
</dt> <dt>

[**POINTER_INFO**](/previous-versions/windows/desktop/api)
</dt> </dl>

 

