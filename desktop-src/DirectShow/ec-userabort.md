---
description: Пользователь завершил воспроизведение.
ms.assetid: 974a9c3e-cfc9-4608-9f98-732aeaa0a752
title: EC_USERABORT (DShow. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d6a546a963a5fe6a2afc0a0d48d086ad59598adb0072e96095a50ac35cf10ba1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119965524"
---
# <a name="ec_userabort"></a>EC \_ усераборт

Пользователь завершил воспроизведение.

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

Отсутствует. Приложение должно решить, следует ли прерывать граф.

## <a name="remarks"></a>Remarks

Этот код события сигнализирует, что пользователь прервал воспроизведение нормального графа. Например, модули подготовки видео отправляют это событие, если пользователь закрывает окно видео.

После отправки этого события фильтр должен отклонить все выборки и не отправлять [**события \_ перерисовки EC**](ec-repaint.md) , пока фильтр не остановится и не будет сброшен.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>DShow. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коды уведомлений о событиях](event-notification-codes.md)
</dt> <dt>

[Уведомление о событии в DirectShow](event-notification-in-directshow.md)
</dt> </dl>

 

 




