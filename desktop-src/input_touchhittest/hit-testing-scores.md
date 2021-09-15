---
title: Оценки проверки попадания касания
description: Следующие константы указывают на возможные результаты проверки попадания для объекта относительно других объектов, пересекающих зону касания.
ms.assetid: EACDE6DB-ADBD-4F0C-8C31-7321AB6A73EA
topic_type:
- apiref
api_name:
- TOUCH_HIT_TESTING_PROXIMITY_CLOSEST
- TOUCH_HIT_TESTING_PROXIMITY_FARTHEST
api_location:
- winuser.h
api_type:
- HeaderDef
ms.topic: article
ms.date: 02/07/2020
ms.openlocfilehash: f6590e7d56c1c9d92f0ff20524b6e4222d8655b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569166"
---
# <a name="touch-hit-testing-scores"></a>Оценки проверки попадания касания

Следующие константы указывают на возможные результаты проверки попадания для объекта относительно других объектов, пересекающих зону касания.

| Константа/значение | Описание |
|---|---|
| **TOUCH_HIT_TESTING_PROXIMITY_CLOSEST** 0x0      | Объект является наиболее вероятной целью.<br/>  |
| **TOUCH_HIT_TESTING_PROXIMITY_FARTHEST** 0xfff | Объект является наименее вероятной целью.<br/> |

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                           |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                            |
| Заголовок<br/>                   | Winuser. h |
