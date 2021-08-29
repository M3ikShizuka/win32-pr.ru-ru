---
title: Сообщение HDM_GETITEMDROPDOWNRECT (Коммктрл. h)
description: Возвращает ограничивающий прямоугольник кнопки разворачивающегося элемента заголовка со стилем ХДФ \_ SPLITBUTTON. Отправляйте это сообщение явным образом или с помощью \_ макроса Жетитемдропдовнрект заголовка.
ms.assetid: d7188dfb-4ffa-4641-b210-2c2ec480ca13
keywords:
- элементы управления Windows сообщений HDM_GETITEMDROPDOWNRECT
topic_type:
- apiref
api_name:
- HDM_GETITEMDROPDOWNRECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f02fa02dd04720a130bf6303927fed64aadc53f4f90acc70a60e2c0cf7afd7ae
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120047174"
---
# <a name="hdm_getitemdropdownrect-message"></a>\_Сообщение ЖЕТИТЕМДРОПДОВНРЕКТ HDM

Возвращает ограничивающий прямоугольник кнопки разворачивающегося элемента заголовка со стилем **ХДФ \_ SPLITBUTTON**. Отправляйте это сообщение явным образом или с помощью макроса [**\_ жетитемдропдовнрект заголовка**](/windows/desktop/api/Commctrl/nf-commctrl-header_getitemdropdownrect) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Отсчитываемый от нуля индекс элемента управления заголовка, для которого требуется получить ограничивающий прямоугольник.

</dd> <dt>

*lParam* \[ в, out\]
</dt> <dd>

Указатель на структуру [**Rect**](/windows/win32/api/windef/ns-windef-rect) , которая получает сведения об ограничивающем прямоугольнике. Отправитель сообщения отвечает за выделение этой структуры. Координаты, возвращаемые в структуре RECT, выражаются относительно родительского элемента управления заголовка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Элемент заголовка должен иметь Style **ХДФ \_ SPLITBUTTON**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Сведения об элементах управления "заголовок"](header-controls.md)
</dt> </dl>

 

 





