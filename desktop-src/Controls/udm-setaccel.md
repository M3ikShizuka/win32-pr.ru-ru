---
title: Сообщение UDM_SETACCEL (Коммктрл. h)
description: Задает ускорение для элемента управления "вверх/вниз".
ms.assetid: af1d0a34-13ba-4bda-82f5-d7afab6bb1ed
keywords:
- элементы управления Windows сообщений UDM_SETACCEL
topic_type:
- apiref
api_name:
- UDM_SETACCEL
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b43ed290ce1668ffcaa9fb086a99ad52e5129ad6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165491"
---
# <a name="udm_setaccel-message"></a>\_Сообщение СЕТАКЦЕЛ UDM

Задает ускорение для элемента управления "вверх/вниз".

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Число структур [**удакцел**](/windows/desktop/api/Commctrl/ns-commctrl-udaccel) , заданных параметром *аакцелс*.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на массив структур [**удакцел**](/windows/desktop/api/Commctrl/ns-commctrl-udaccel) , содержащих сведения об ускорении. Элементы должны быть отсортированы в порядке возрастания на основе элемента **NSEC** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_UDM**](udm-getaccel.md)
</dt> </dl>

 

 





