---
title: Сообщение UDM_GETACCEL (Коммктрл. h)
description: Получает сведения о ускорении для элемента управления "вверх/вниз".
ms.assetid: 794538d6-ca01-4f05-82d1-ce7bc0f76f64
keywords:
- элементы управления Windows сообщений UDM_GETACCEL
topic_type:
- apiref
api_name:
- UDM_GETACCEL
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b86a9740e59631b737453763a10ccb9820056d95
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165524"
---
# <a name="udm_getaccel-message"></a>\_Сообщение о неполучении UDM

Получает сведения о ускорении для элемента управления "вверх/вниз".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Число элементов в массиве, заданном параметром *lParam*.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на массив структур [**удакцел**](/windows/desktop/api/Commctrl/ns-commctrl-udaccel) , которые получают сведения о ускорении.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение — это число ускорителей, установленных в данный момент для элемента управления.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_СЕТАКЦЕЛ UDM**](udm-setaccel.md)
</dt> </dl>

 

 





