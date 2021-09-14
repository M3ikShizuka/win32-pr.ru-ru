---
title: Сообщение BCM_SETTEXTMARGIN (Коммктрл. h)
description: '\_Сообщение СЕТТЕКСТМАРГИН BCM задает поля для рисования текста в элементе управления "Кнопка".'
ms.assetid: 0798b1c5-7db4-46c6-8881-4c847abc7460
keywords:
- элементы управления Windows сообщений BCM_SETTEXTMARGIN
topic_type:
- apiref
api_name:
- BCM_SETTEXTMARGIN
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4fb6653007c155a508ce4da899a7be0d8ff2ab2d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968741"
---
# <a name="bcm_settextmargin-message"></a>\_Сообщение СЕТТЕКСТМАРГИН BCM

Сообщение **\_ сеттекстмаргин BCM** задает поля для рисования текста в элементе управления "Кнопка".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**Rect**](/previous-versions//dd162897(v=vs.85)) , указывающую поля, используемые для рисования текста.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если сообщение завершается с ошибкой, возвращается **значение true**. В противном случае возвращается **значение false**.

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

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

[**Кнопка " \_ сеттекстмаргин"**](/windows/desktop/api/Commctrl/nf-commctrl-button_settextmargin)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Кнопки](buttons.md)
</dt> </dl>

 

