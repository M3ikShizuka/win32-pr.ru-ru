---
description: Уведомляет приложение, когда выбранному РЕДАКТОРу требуется информация о окне композиции. Приложение получает эту команду через \_ сообщение запроса WM IME \_ с набором параметров, как показано ниже.
ms.assetid: 08fd7119-d225-4a78-b2cd-8b58887c9139
title: Код уведомления IMR_COMPOSITIONWINDOW (IMM. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8fc5f1f45652a2f58386a50284e3bf2cfec182c6f4ad89641dcc27a63cf12b78
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "117810057"
---
# <a name="imr_compositionwindow-notification-code"></a>\_Код уведомления КОМПОСИТИОНВИНДОВ IMR

Уведомляет приложение, когда выбранному РЕДАКТОРу требуется информация о окне композиции. Приложение получает эту команду через сообщение [**запроса WM \_ IME \_**](wm-ime-request.md) с набором параметров, как показано ниже.


```C++
LRESULT IMR_COMPOSITIONWINDOW
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="wParam"></span><span id="wparam"></span><span id="WPARAM"></span>*wParam*
</dt> <dd>

Задайте значение IMR \_ компоситионвиндов.

</dd> <dt>

<span id="lParam"></span><span id="lparam"></span><span id="LPARAM"></span>*lParam*
</dt> <dd>

Указатель на буфер, содержащий структуру [**компоситионформ**](/windows/win32/api/imm/ns-imm-compositionform) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Функция возвращает ненулевое значение, если приложение заполняет структуру [**компоситионформ**](/windows/win32/api/imm/ns-imm-compositionform) . В противном случае команда возвращает значение 0.

## <a name="remarks"></a>Remarks

Эта команда может быть отправлена редактором IME в окно, которое очистило \_ флаг ISC шовуикомпоситионвиндов в обработчике сообщений [**\_ \_ SETCONTEXT редактора IME**](wm-ime-setcontext.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                 |
| Заголовок<br/>                   | <dl> <dt>Imm. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Диспетчер метода ввода](input-method-manager.md)
</dt> <dt>

[Команды диспетчера методов ввода](input-method-manager-commands.md)
</dt> <dt>

[**компоситионформ**](/windows/win32/api/imm/ns-imm-compositionform)
</dt> <dt>

[**\_запрос IME \_ WM**](wm-ime-request.md)
</dt> <dt>

[**\_SETCONTEXT IME \_ WM**](wm-ime-setcontext.md)
</dt> </dl>

 

 




