---
title: Сообщение CB_GETMINVISIBLE (Коммктрл. h)
description: Возвращает минимальное число видимых элементов в раскрывающемся списке поля со списком.
ms.assetid: 9861358a-1ef9-4d78-8ec8-561b97f3f18e
keywords:
- элементы управления Windows сообщений CB_GETMINVISIBLE
topic_type:
- apiref
api_name:
- CB_GETMINVISIBLE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3dcf4fe5088d9c994e232a64ba16bbddf11b0d48
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174188"
---
# <a name="cb_getminvisible-message"></a>\_Сообщение ЖЕТМИНВИСИБЛЕ CB

Возвращает минимальное число видимых элементов в раскрывающемся списке поля со списком.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение — это минимальное число видимых элементов.

## <a name="remarks"></a>Remarks

Если число элементов в раскрывающемся списке больше минимального, в поле со списком используется полоса прокрутки.

Это сообщение пропускается, если элемент управления "поле со списком" имеет стиль [**CBS \_ ноинтегралхеигхт**](combo-box-styles.md).

Чтобы использовать **CB \_ жетминвисибле**, приложение должно указать comctl32.dll версии 6 в манифесте. Дополнительные сведения см. в разделе [Включение визуальных стилей](cookbook-overview.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**\_СЕТМИНВИСИБЛЕ CB**](cb-setminvisible.md)
</dt> <dt>

[**Поле со списком \_ жетминвисибле**](/windows/desktop/api/Commctrl/nf-commctrl-combobox_getminvisible)
</dt> </dl>

 

 





