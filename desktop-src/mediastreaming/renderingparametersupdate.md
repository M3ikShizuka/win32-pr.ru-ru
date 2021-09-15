---
title: Событие Рендерингпараметерсупдате
description: Возникает при обновлении любого из набора параметров элемента управления отрисовки в ДМР.
ms.assetid: 863ca879-a420-43d6-9ac8-94f8303bb759
keywords:
- API потоковой передачи мультимедиа для события Рендерингпараметерсупдате
topic_type:
- apiref
api_name:
- RenderingParametersUpdate
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 35e4898bae876babb0e5fbc1c4b9760eec6a9b62
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571655"
---
# <a name="renderingparametersupdate-event"></a>Событие Рендерингпараметерсупдате

Возникает при обновлении любого из набора параметров элемента управления отрисовки в ДМР.

## <a name="syntax"></a>Синтаксис


```C++
void RenderingParametersUpdate();
```



## <a name="parameters"></a>Параметры

У этого события нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Для обработки уведомлений из этого события Зарегистрируйте функцию обработчика событий [**рендерингпараметерсупдатехандлер**](/previous-versions/windows/desktop/legacy/hh828994(v=vs.85)) с помощью метода [**Add \_ рендерингпараметерсупдате**](/previous-versions/windows/desktop/api/windows.media.streaming/nf-windows-media-streaming-imediarenderer-add_renderingparametersupdate) . Чтобы отменить регистрацию обработчика событий, используйте метод [**Remove \_ рендерингпараметерсупдате**](/previous-versions/windows/desktop/api/windows.media.streaming/nf-windows-media-streaming-imediarenderer-remove_renderingparametersupdate) .

 

 