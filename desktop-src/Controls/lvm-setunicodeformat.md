---
title: Сообщение LVM_SETUNICODEFORMAT (Коммктрл. h)
description: LVM_SETUNICODEFORMAT сообщение — задает флаг формата символов Юникода для элемента управления.
ms.assetid: e332ae88-821f-4341-a98d-59d8a01a126f
keywords:
- элементы управления Windows сообщений LVM_SETUNICODEFORMAT
topic_type:
- apiref
api_name:
- LVM_SETUNICODEFORMAT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bb0f700cd057bc77eddc699404f37b19a6cc9c39
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362649"
---
# <a name="lvm_setunicodeformat-message"></a>\_Сообщение LVM сетуникодеформат

Задает флаг формата символов Юникода для элемента управления. Это сообщение позволяет изменить кодировку, используемую элементом управления во время выполнения, вместо того, чтобы повторно создавать элемент управления. Это сообщение можно отправить явным образом или использовать макрос [**\_ сетуникодеформат ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_setunicodeformat) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Определяет кодировку, используемую элементом управления. Если это значение не равно нулю, элемент управления будет использовать символы Юникода. Если это значение равно нулю, элемент управления будет использовать символы ANSI.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает предыдущий флаг формата Юникода для элемента управления.

## <a name="remarks"></a>Комментарии

Обсуждение этого сообщения см. в примечаниях по [**CCM \_ сетуникодеформат**](ccm-setunicodeformat.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**LVM \_ жетуникодеформат**](lvm-getunicodeformat.md)
</dt> </dl>

 

 





