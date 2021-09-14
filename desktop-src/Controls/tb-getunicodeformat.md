---
title: Сообщение TB_GETUNICODEFORMAT (Коммктрл. h)
description: TB_GETUNICODEFORMAT сообщение — получает флаг формата символов Юникода для элемента управления.
ms.assetid: aadce646-daf1-4f1e-9171-2aeac12d3484
keywords:
- элементы управления Windows сообщений TB_GETUNICODEFORMAT
topic_type:
- apiref
api_name:
- TB_GETUNICODEFORMAT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4beb5a5ff0b71dd76c85db2788d9dc91aa9f4957
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166739"
---
# <a name="tb_getunicodeformat-message"></a>\_Сообщение ЖЕТУНИКОДЕФОРМАТ ТБ

Возвращает флаг формата символов Юникода для элемента управления.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает флаг формата Юникода для элемента управления. Если это значение не равно нулю, то элемент управления использует символы Юникода. Если это значение равно нулю, то элемент управления использует символы ANSI.

## <a name="remarks"></a>Remarks

Обсуждение этого сообщения см. в примечаниях по [**CCM \_ жетуникодеформат**](ccm-getunicodeformat.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_СЕТУНИКОДЕФОРМАТ ТБ**](tb-setunicodeformat.md)
</dt> </dl>

 

 





