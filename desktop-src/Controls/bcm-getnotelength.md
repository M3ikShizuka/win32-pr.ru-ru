---
title: Сообщение BCM_GETNOTELENGTH (Коммктрл. h)
description: Возвращает длину текста примечания, который может отображаться в описании кнопки ссылки на команду. Отправляйте это сообщение явным образом или с помощью \_ макроса кнопки жетнотеленгс.
ms.assetid: 62385485-b553-47e9-9f15-696cc4694752
keywords:
- элементы управления Windows сообщений BCM_GETNOTELENGTH
topic_type:
- apiref
api_name:
- BCM_GETNOTELENGTH
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1b33c5245778481033bd97326c3d66a40bf03210
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170124"
---
# <a name="bcm_getnotelength-message"></a>\_Сообщение ЖЕТНОТЕЛЕНГС BCM

Возвращает длину текста примечания, который может отображаться в описании кнопки ссылки на команду. Отправляйте это сообщение явным образом или с помощью макроса [**кнопки \_ жетнотеленгс**](/windows/desktop/api/Commctrl/nf-commctrl-button_getnotelength) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает длину текста примечания в **вчарс**, не включая завершающий **нуль**-символ, или нуль, если текст примечания отсутствует.

## <a name="remarks"></a>Remarks

Начиная с Comctl32 DLL версии 6,01, кнопки ссылки на команды могут иметь Примечание. Сведения о версиях DLL см. в разделе [общие версии элементов управления](common-control-versions.md).

Сообщение **BCM \_ жетнотеленгс** работает только с стилями кнопки [**BS \_ коммандлинк**](button-styles.md) и [**BS \_ дефкоммандлинк**](button-styles.md) .

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

 

 





