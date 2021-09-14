---
title: Сообщение TBM_SETSELEND (Коммктрл. h)
description: Задает конечную логическую точку текущего выделенного диапазона в TrackBar. Это сообщение пропускается, если значение TrackBar не имеет \_ стиля TBS енаблеселранже.
ms.assetid: 1feec14c-1607-49d5-a147-af2443f82dc1
keywords:
- элементы управления Windows сообщений TBM_SETSELEND
topic_type:
- apiref
api_name:
- TBM_SETSELEND
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 146446df4daf8e8ac7c0f3499149ba0f46940880
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166427"
---
# <a name="tbm_setselend-message"></a>\_Сообщение ТБМ сетселенд

Задает конечную логическую точку текущего выделенного диапазона в TrackBar. Это сообщение пропускается, если значение TrackBar не имеет стиля [**TBS \_ енаблеселранже**](trackbar-control-styles.md) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Флаг перерисовки. Если этот параметр имеет **значение true**, сообщение перерисовывается после установки диапазона выбора. Если этот параметр имеет **значение false**, то сообщение задает диапазон выбора, но не перерисовывает линейку.

</dd> <dt>

*lParam* 
</dt> <dd>

Конечная логическая позиция диапазона выбора.

</dd> </dl>

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

**Ссылка**
</dt> <dt>

[**ТБМ \_ жетселенд**](tbm-getselend.md)
</dt> <dt>

[**ТБМ \_ жетселстарт**](tbm-getselstart.md)
</dt> <dt>

[**ТБМ \_ сетсел**](tbm-setsel.md)
</dt> <dt>

[**ТБМ \_ сетселстарт**](tbm-setselstart.md)
</dt> </dl>

 

 





