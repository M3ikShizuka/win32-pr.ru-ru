---
title: Системмонитор Коллектсампле, метод
description: Выбирает значение для каждого счетчика в объекте Counters.
ms.assetid: 4c91c759-597f-4aa8-aa77-eb181616e8b0
keywords:
- Метод Коллектсампле Сисмон
- Метод Коллектсампле Сисмон, интерфейс Системмонитор
- Интерфейс Системмонитор Сисмон, метод Коллектсампле
topic_type:
- apiref
api_name:
- SystemMonitor.CollectSample
api_location:
- Sysmon.ocx
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0e1c269d044c17a2ec1322fa969e0c86f468a901
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056781"
---
# <a name="systemmonitorcollectsample-method"></a>Метод Системмонитор:: Коллектсампле

Выбирает значение для каждого счетчика в объекте [**Counters**](counters.md) .

## <a name="syntax"></a>Синтаксис


```VB
Sub CollectSample()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

Вызывайте **коллектсампле** только в том случае, если [**Мануалупдате**](systemmonitor-manualupdate.md) имеет значение true, а значения счетчика выборки из текущей активности компьютера не используют этот метод при выборке из файла журнала. Диаграмма или отчет будут обновлены новым значением. Обратите внимание, что для диаграмм некоторых типов диаграмм требуются два образца, например линейный график.

Чтобы получить уведомление при сборе примера, реализуйте событие [**онсамплеколлектед**](-systemmonitor-onsamplecollected.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Counters**](counters.md)
</dt> <dt>

[**системмонитор**](systemmonitor.md)
</dt> </dl>

 

 





