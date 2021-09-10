---
title: Сообщение WM_CAP_SET_CALLBACK_YIELD (VFW. h)
description: Сообщение о выдачей \_ \_ \_ обратного вызова Set крепления WM \_ устанавливает функцию обратного вызова в приложении. Авикап вызывает эту процедуру, когда окно записи выдается во время потоковой записи. Это сообщение можно отправить явно или с помощью макроса Капсеткаллбаккониелд.
ms.assetid: d978dc3b-4336-46a4-85ae-7d588a63489b
keywords:
- сообщение WM_CAP_SET_CALLBACK_YIELD Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_SET_CALLBACK_YIELD
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b95c9ba0be7a0abeb99c0590e255adb0bd442343
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371499"
---
# <a name="wm_cap_set_callback_yield-message"></a>\_Сообщение о \_ \_ выдает ответ обратного вызова Set крепления WM \_

Сообщение о выдачей **\_ \_ \_ обратного вызова \_ Set крепления WM** устанавливает функцию обратного вызова в приложении. Авикап вызывает эту процедуру, когда окно записи выдается во время потоковой записи. Это сообщение можно отправить явно или с помощью макроса [**капсеткаллбаккониелд**](/windows/desktop/api/Vfw/nf-vfw-capsetcallbackonyield) .


```C++
WM_CAP_SET_CALLBACK_YIELD 
wParam = (WPARAM) 0; 
lParam = (LPARAM) (LPVOID) (fpProc); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="fpProc"></span><span id="fpproc"></span><span id="FPPROC"></span>*фппрок*
</dt> <dd>

Указатель на функцию обратного вызова yield типа [**капиелдкаллбакк**](/windows/desktop/api/Vfw/nc-vfw-capyieldcallback). Укажите **значение NULL** для этого параметра, чтобы отключить ранее установленную функцию обратного вызова yield.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** в случае успеха или **false** , если выполняется захват потоковой передачи или однокадровый сеанс записи.

## <a name="remarks"></a>Remarks

При необходимости приложения могут устанавливать функцию обратного вызова yield. Функция обратного вызова yield вызывается по крайней мере один раз для каждого видеокадра, захваченного при захвате потоковой передачи. Если установлена функция обратного вызова yield, она будет вызываться независимо от состояния элемента **Фиелд** структуры [**каптурепармс**](/windows/win32/api/vfw/ns-vfw-captureparms) .

Если используется функция обратного вызова yield, ее необходимо установить перед запуском сеанса записи, и она должна оставаться включенной в течение сеанса. Его можно отключить после завершения потоковой записи.

Приложения обычно выполняют некоторый тип обработки сообщений в функции обратного вызова, состоящей из цикла [PeekMessage](/windows/win32/api/winuser/nf-winuser-peekmessagea), [TranslateMessage](/windows/win32/api/winuser/nf-winuser-translatemessage), [DispatchMessage](/windows/win32/api/winuser/nf-winuser-dispatchmessage) , как в цикле обработки сообщений функции [WinMain](/windows/win32/api/winbase/nf-winbase-winmain) . Функция обратного вызова yield также должна фильтровать и удалять сообщения, которые могут вызвать проблемы повторного входа.

Приложение обычно возвращает **значение true** в процедуре yield, чтобы продолжить потоковую передачу. Если функция обратного вызова Yield возвращает **значение false**, окно отслеживания останавливает процесс отслеживания.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> <dt>

[Сообщения видеозаписи](video-capture-messages.md)
</dt> </dl>

 

