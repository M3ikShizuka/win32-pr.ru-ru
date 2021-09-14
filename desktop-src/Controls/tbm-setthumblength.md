---
title: Сообщение TBM_SETTHUMBLENGTH (Коммктрл. h)
description: Задает длину ползунка в TrackBar. Это сообщение пропускается, если значение TrackBar не имеет \_ стиля TBS FIXEDLENGTH.
ms.assetid: 027fe341-a60a-4dbe-a48a-5ddaadef0b4a
keywords:
- элементы управления Windows сообщений TBM_SETTHUMBLENGTH
topic_type:
- apiref
api_name:
- TBM_SETTHUMBLENGTH
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0d4ac33d2df43a267766e14ab95fb9729692bbee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166419"
---
# <a name="tbm_setthumblength-message"></a>\_Сообщение ТБМ сетсумбленгс

Задает длину ползунка в TrackBar. Это сообщение пропускается, если значение TrackBar не имеет стиля [**TBS \_ FIXEDLENGTH**](trackbar-control-styles.md) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Длина ползунка в пикселях.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ТБМ \_ жетсумбленгс**](tbm-getthumblength.md)
</dt> </dl>

 

 





