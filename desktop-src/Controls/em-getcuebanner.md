---
title: Сообщение EM_GETCUEBANNER (Коммктрл. h)
description: Возвращает текст, который отображается как текстовая подсказка или Совет в элементе управления "поле ввода".
ms.assetid: 311b783a-cd78-440f-bfc2-f5108ae7d1f8
keywords:
- элементы управления Windows сообщений EM_GETCUEBANNER
topic_type:
- apiref
api_name:
- EM_GETCUEBANNER
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5d28d4aeea5a206c74f2e6b41cee27b5073448ba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054443"
---
# <a name="em_getcuebanner-message"></a>\_Сообщение ЖЕТКУЕБАННЕР EM

Возвращает текст, который отображается как текстовая подсказка или Совет в элементе управления "поле ввода".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Указатель на буфер Юникода, который получает текстовый набор в качестве текстовой подсказки. Вызывающий объект отвечает за выделение буфера.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd>

Размер буфера, на который указывает *wParam* в **вчарс**, включая завершающее **значение NULL**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** в случае успеха или **false** в противном случае.

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

[**Изменить \_ жеткуебаннертекст**](/windows/desktop/api/Commctrl/nf-commctrl-edit_getcuebannertext)
</dt> </dl>

 

 





