---
title: Сообщение MCM_SETSELRANGE (Коммктрл. h)
description: Задает для элемента управления "месячный календарь" определенный диапазон дат. Это сообщение можно отправить явным образом или с помощью \_ макроса монскал сетселранже.
ms.assetid: 750b0c83-6baa-4caa-a738-feae8751a70e
keywords:
- элементы управления Windows сообщений MCM_SETSELRANGE
topic_type:
- apiref
api_name:
- MCM_SETSELRANGE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1cdf6708aa382abfa92562aa55943c06180d0231cff568b74de380416e48731a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119018982"
---
# <a name="mcm_setselrange-message"></a>\_Сообщение MCM сетселранже

Задает для элемента управления "месячный календарь" определенный диапазон дат. Это сообщение можно отправить явным образом или с помощью макроса [**монскал \_ сетселранже**](/windows/desktop/api/Commctrl/nf-commctrl-monthcal_setselrange) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на массив элементов [**SYSTEMTIME**](/windows/desktop/api/minwinbase/ns-minwinbase-systemtime) с двумя элементами, содержащий сведения о дате, представляющие ограничения выбора. Первая выбранная дата должна быть указана в *лпсистимеаррай* \[ 0 \] , а последняя выбранная дата должна быть указана в *лпсистимеаррай* \[ 1 \] .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение в случае успеха или ноль в противном случае. Это сообщение не будет выполнено, если применяется к элементу управления "месячный календарь", который не использует многоэлементный стиль [**MCS \_**](month-calendar-control-styles.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Время в элементе управления ' календарь на месяц '](month-calendar-controls.md)
</dt> </dl>

 

