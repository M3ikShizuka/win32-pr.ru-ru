---
title: Сообщение BCM_GETSPLITINFO (Коммктрл. h)
description: Возвращает сведения для элемента управления "кнопка разворачивающейся кнопки". Отправляйте это сообщение явным образом или с помощью \_ макроса кнопки жетсплитинфо.
ms.assetid: d608440d-b8d8-4e32-9128-08b7566b185c
keywords:
- элементы управления Windows сообщений BCM_GETSPLITINFO
topic_type:
- apiref
api_name:
- BCM_GETSPLITINFO
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 162c5522fcb432e3d512f688ae24aa12d4d0d8e1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170128"
---
# <a name="bcm_getsplitinfo-message"></a>\_Сообщение ЖЕТСПЛИТИНФО BCM

Возвращает сведения для элемента управления "кнопка разворачивающейся кнопки". Отправляйте это сообщение явным образом или с помощью макроса [**кнопки \_ жетсплитинфо**](/windows/desktop/api/Commctrl/nf-commctrl-button_getsplitinfo) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* \[ в, out\]
</dt> <dd>

Указатель на структуру [**кнопки \_ сплитинфо**](/windows/win32/api/commctrl/ns-commctrl-button_splitinfo) для получения сведений о кнопке. Вызывающий объект отвечает за выделение памяти для структуры. Установите элемент **маски** этой структуры, чтобы определить, какие сведения следует получить.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Это сообщение используется только с стилями кнопки " [**BS \_**](button-styles.md) " и " [**BS \_ дефсплитбуттон**](button-styles.md) ".

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[Стили кнопок](button-styles.md)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Типы кнопок](button-types-and-styles.md)
</dt> </dl>

 

 





