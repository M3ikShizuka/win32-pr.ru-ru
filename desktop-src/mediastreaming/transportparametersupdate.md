---
title: Событие Транспортпараметерсупдате
description: Происходит при каждом обновлении любого из наборов параметров транспорта в ДМР.
ms.assetid: df9256ca-6c59-462c-b32f-4653546db384
keywords:
- API потоковой передачи мультимедиа для события Транспортпараметерсупдате
topic_type:
- apiref
api_name:
- TransportParametersUpdate
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 58df04862275af5da8714f8a954dc5b127f833f2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127252472"
---
# <a name="transportparametersupdate-event"></a>Событие Транспортпараметерсупдате

Происходит при каждом обновлении любого из наборов параметров транспорта в ДМР.

## <a name="syntax"></a>Синтаксис


```C++
void TransportParametersUpdate();
```



## <a name="parameters"></a>Параметры

У этого события нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Для обработки уведомлений из этого события Зарегистрируйте функцию обработчика событий [**транспортпараметерсупдатехандлер**](/previous-versions/windows/desktop/legacy/hh829007(v=vs.85)) с помощью метода [**Add \_ транспортпараметерсупдате**](/previous-versions/windows/desktop/api/windows.media.streaming/nf-windows-media-streaming-imediarenderer-add_transportparametersupdate) . Чтобы отменить регистрацию обработчика событий, используйте метод [**Remove \_ транспортпараметерсупдате**](/previous-versions/windows/desktop/api/windows.media.streaming/nf-windows-media-streaming-imediarenderer-remove_transportparametersupdate) .

 

 