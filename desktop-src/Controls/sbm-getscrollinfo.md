---
title: Сообщение SBM_GETSCROLLINFO (Winuser. h)
description: '\_Для получения параметров полосы прокрутки отправляется сообщение СБМ жетскроллинфо.'
ms.assetid: 3b43430f-b55f-43ec-8558-baf5c953064f
keywords:
- элементы управления Windows сообщений SBM_GETSCROLLINFO
topic_type:
- apiref
api_name:
- SBM_GETSCROLLINFO
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c4cb05b05ba2686d755c5fa34adcff0016433346
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167076"
---
# <a name="sbm_getscrollinfo-message"></a>\_Сообщение СБМ жетскроллинфо

Для получения параметров полосы прокрутки отправляется сообщение **СБМ \_ жетскроллинфо** .

Приложения не должны отсылать это сообщение напрямую. Вместо этого они должны использовать функцию [**жетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-getscrollinfo) . Окно получает это сообщение через функцию [*WindowProc*](/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)) . Приложения, которые реализуют пользовательский элемент управления "полоса прокрутки", должны отвечать на эти сообщения, чтобы функция **жетскроллинфо** работала правильно.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**скроллинфо**](/windows/win32/api/winuser/ns-winuser-scrollinfo) . Перед вызовом [**жетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-getscrollinfo)задайте для элемента **кбсизе** структуры значение **sizeof**(**скроллинфо**) и установите элемент **фмаск** , чтобы указать параметры полосы прокрутки для извлечения. Перед возвратом сообщение копирует указанные параметры в соответствующие члены структуры.

Элемент **фмаск** может иметь одно или несколько из следующих значений.



| Значение                                                                                                                                                      | Значение                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| <span id="SIF_ALL"></span><span id="sif_all"></span><dl> <dt>**SIF \_ все**</dt> </dl>                | Сочетание страницы SIF \_ , SIF \_ POS, SIF \_ Range и SIF \_ траккпос.<br/>       |
| <span id="SIF_PAGE"></span><span id="sif_page"></span><dl> <dt>**\_страница SIF**</dt> </dl>             | Копирует страницу прокрутки в элемент Нпаже.<br/>                              |
| <span id="SIF_POS"></span><span id="sif_pos"></span><dl> <dt>**SIF \_ POS**</dt> </dl>                | Копирует расположение прокрутки в элемент nPos. <br/>                          |
| <span id="SIF_RANGE"></span><span id="sif_range"></span><dl> <dt>**\_диапазон SIF**</dt> </dl>          | Копирует диапазон прокрутки в элементы Nмин. и Nмакс.. <br/>                   |
| <span id="SIF_TRACKPOS"></span><span id="sif_trackpos"></span><dl> <dt>**SIF \_ траккпос**</dt> </dl> | Копирует текущую отслеживаемую точку прокрутки в элемент Нтраккпос.<br/> |



 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение получает какие-либо значения, возвращается значение **true**. в противном случае — **false**.

## <a name="remarks"></a>Remarks

Сообщения, указывающие расположение полосы прокрутки, [**WM \_ HSCROLL**](wm-hscroll.md) и [**WM \_ VSCROLL**](wm-vscroll.md), содержат только 16 бит данных о положении. Однако структура [**скроллинфо**](/windows/win32/api/winuser/ns-winuser-scrollinfo) , используемая **СБМ \_ жетскроллинфо**, [**СБМ \_ сетскроллинфо**](sbm-setscrollinfo.md), [**жетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-getscrollinfo)и [**сетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-setscrollinfo) , предоставляет 32 бит для расположения данных в полосе прокрутки. Эти сообщения и функции можно использовать при обработке сообщений **WM \_ HSCROLL** или **WM \_ VSCROLL** для получения данных о положении полосы прокрутки 32 бит.

Чтобы получить 32-разрядную точку прокрутки (Thumb) во время выполнения \_ кода запроса SB сумбтракк [**\_ HSCROLL**](wm-hscroll.md) или [**WM \_ VSCROLL**](wm-vscroll.md) , отправьте **СБМ \_ жетскроллинфо** со \_ значением SIF траккпос в **фмаск** -члене структуры [**скроллинфо**](/windows/win32/api/winuser/ns-winuser-scrollinfo) . Сообщение возвращает точку отслеживания ползунка в элементе **нтраккпос** структуры **скроллинфо** . Это позволяет получить расположение поля прокрутки при его перемещении пользователем. Кроме того, можно использовать функцию [**жетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-getscrollinfo) для получения той же информации.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылка**
</dt> <dt>

[**жетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-getscrollinfo)
</dt> <dt>

[**СБМ \_ сетскроллинфо**](sbm-setscrollinfo.md)
</dt> <dt>

[**скроллинфо**](/windows/win32/api/winuser/ns-winuser-scrollinfo)
</dt> <dt>

[**сетскроллинфо**](/windows/desktop/api/Winuser/nf-winuser-setscrollinfo)
</dt> </dl>

 

