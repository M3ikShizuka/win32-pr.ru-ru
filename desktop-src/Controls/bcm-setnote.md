---
title: Сообщение BCM_SETNOTE (Коммктрл. h)
description: Задает текст примечания, связанного с кнопкой ссылки на команду. Это сообщение можно отправить явным образом или воспользоваться \_ макросом кнопки сетноте.
ms.assetid: c167072a-8207-4744-ac66-247141d726ab
keywords:
- элементы управления Windows сообщений BCM_SETNOTE
topic_type:
- apiref
api_name:
- BCM_SETNOTE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f544a7fb9dd89346cc2aa9725d36122746a8f608
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968742"
---
# <a name="bcm_setnote-message"></a>\_Сообщение СЕТНОТЕ BCM

Задает текст примечания, связанного с кнопкой ссылки на команду. Это сообщение можно отправить явным образом или воспользоваться макросом [**кнопки \_ сетноте**](/windows/desktop/api/Commctrl/nf-commctrl-button_setnote) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на строку типа **WCHAR** , заканчивающуюся нулем, которая содержит Примечание.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Комментарии

Начиная с Comctl32 DLL версии 6,01, кнопки ссылки на команды могут иметь Примечание.

Сообщение **BCM \_ сетноте** работает только с стилями кнопки [**BS \_ коммандлинк**](button-styles.md) и [**BS \_ дефкоммандлинк**](button-styles.md) .

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

 

 





