---
title: Креатемедиарендерероператион. Completed, свойство
description: Возвращает или задает обработчик событий, вызываемый при завершении асинхронной операции, запущенной Креатемедиарендерерасинк или Креатемедиарендерерфромбасикдевицеасинк.
ms.assetid: B62CF929-13D0-4665-89E4-DEC48A38DDF7
keywords:
- Законченное свойство потоковой передачи мультимедиа API
- Завершенное свойство потоковой передачи мультимедиа API, интерфейс Креатемедиарендерероператион
- API потоковой передачи мультимедиа интерфейса Креатемедиарендерероператион, завершенное свойство
topic_type:
- apiref
api_name:
- CreateMediaRendererOperation.Completed
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 86f2a0f33bfe00b65dc6e2e8a77d1e29e0ad4ea05888d6dba86797898bc8cfb3
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119952784"
---
# <a name="createmediarendereroperationcompleted-property"></a>Креатемедиарендерероператион. Completed, свойство

Возвращает или задает обработчик событий, вызываемый при завершении асинхронной операции, запущенной [**креатемедиарендерерасинк**](imediarendererfactory-createmediarendererasync.md) или [**креатемедиарендерерфромбасикдевицеасинк**](imediarendererfactory-createmediarendererfrombasicdeviceasync.md) .

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_Completed(
  [in]  ICreateMediaRendererCompletedHandler value
);

HRESULT get_Completed(
  [out] ICreateMediaRendererCompletedHandler *value
);
```



## <a name="property-value"></a>Значение свойства

Обработчик событий.

## <a name="see-also"></a>См. также

<dl> <dt>

[**креатемедиарендерероператион**](createmediarendereroperation.md)
</dt> </dl>

 

 




