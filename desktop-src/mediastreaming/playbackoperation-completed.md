---
title: Плайбаккоператион. Completed, свойство
description: Возвращает или задает обработчик событий, вызываемый при завершении асинхронной операции, запущенной одним из методов воспроизведения Медиарендерер.
ms.assetid: E8F8D3FC-C31F-485C-A30B-2457F4B1DE82
keywords:
- Законченное свойство потоковой передачи мультимедиа API
- Завершенное свойство потоковой передачи мультимедиа API, интерфейс Плайбаккоператион
- API потоковой передачи мультимедиа интерфейса Плайбаккоператион, завершенное свойство
topic_type:
- apiref
api_name:
- PlaybackOperation.Completed
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 65721977b535a799d3dfa679b026b2d1d06b3eb9d449e487ceaeeeacb135d625
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119034512"
---
# <a name="playbackoperationcompleted-property"></a>Плайбаккоператион. Completed, свойство

Возвращает или задает обработчик событий, вызываемый при завершении асинхронной операции, запущенной одним из методов воспроизведения [**медиарендерер**](mediarenderer.md) .

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_Completed(
  [in]  PlaybackOperationCompletedHandler *value
);

HRESULT get_Completed(
  [out] PlaybackOperationCompletedHandler **value
);
```



## <a name="property-value"></a>Значение свойства

Обработчик событий.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**плайбаккоператион**](playbackoperation.md)
</dt> </dl>

 

 




