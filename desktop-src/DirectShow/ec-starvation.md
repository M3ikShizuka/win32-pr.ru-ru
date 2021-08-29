---
description: Фильтр не получает достаточно данных.
ms.assetid: c9cdfe46-02bb-4ea9-ac58-7d63e03c26d8
title: EC_STARVATION (DShow. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3405bcf67db3e7dbfead0d841b542e155175bcabdd8283b5a5f76f4195cdd714
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119905784"
---
# <a name="ec_starvation"></a>нехватка ресурсов EC \_

Фильтр не получает достаточно данных.

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lParam1"></span><span id="lparam1"></span><span id="LPARAM1"></span>*lParam1*
</dt> <dd>

Ноль.

</dd> <dt>

<span id="lParam2"></span><span id="lparam2"></span><span id="LPARAM2"></span>*lParam2*
</dt> <dd>

Ноль.

</dd> </dl>

## <a name="default-action"></a>Действие по умолчанию

Событие не отправляется в приложение. Если граф фильтра выполняется, диспетчер графа фильтров приостанавливает граф и ждет завершения паузы. Затем он снова запускает граф. Фильтр, отправляющий событие, не должен завершать его работу до тех пор, пока не пойдет достаточно данных для возобновления. Если граф фильтра не работает, диспетчер графа фильтров игнорирует это событие.

## <a name="remarks"></a>Remarks

Средство синтаксического анализа или фильтр источников может отправить это событие, если поступают слишком мало данных.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>DShow. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Коды уведомлений о событиях](event-notification-codes.md)
</dt> <dt>

[Уведомление о событии в DirectShow](event-notification-in-directshow.md)
</dt> </dl>

 

 




