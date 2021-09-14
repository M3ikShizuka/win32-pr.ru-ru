---
title: Сообщение TCM_SETUNICODEFORMAT (Коммктрл. h)
description: TCM_SETUNICODEFORMAT сообщение — задает флаг формата символов Юникода для элемента управления.
ms.assetid: 4a9bacfc-d1b7-432a-9b61-b0fe18576679
keywords:
- элементы управления Windows сообщений TCM_SETUNICODEFORMAT
topic_type:
- apiref
api_name:
- TCM_SETUNICODEFORMAT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c2b84f944be9bd20897d25e4b111f55ced558a43
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166183"
---
# <a name="tcm_setunicodeformat-message"></a>\_Сообщение СЕТУНИКОДЕФОРМАТ TCM

Задает флаг формата символов Юникода для элемента управления. Это сообщение позволяет изменить кодировку, используемую элементом управления во время выполнения, вместо того, чтобы повторно создавать элемент управления. Это сообщение можно отправить явным образом или использовать макрос [**табктрл \_ сетуникодеформат**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_setunicodeformat) .

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

## <a name="remarks"></a>Remarks

Обсуждение этого сообщения см. в примечаниях по [**CCM \_ сетуникодеформат**](ccm-setunicodeformat.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ЖЕТУНИКОДЕФОРМАТ TCM**](tcm-getunicodeformat.md)
</dt> </dl>

 

 





