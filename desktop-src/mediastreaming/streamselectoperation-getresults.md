---
title: Стреамселектоператион. results, метод
description: Возвращает результаты асинхронной операции, запущенной Селектбестстреамасинк.
ms.assetid: 2D9887E7-17C8-4161-984F-FA44591D2052
keywords:
- API потоковой передачи мультимедиа метода
- API потоковой передачи мультимедиа, интерфейс Стреамселектоператион
- API потоковой передачи мультимедиа интерфейса Стреамселектоператион, метод Results
topic_type:
- apiref
api_name:
- StreamSelectOperation.GetResults
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: c52479949413d32ca54654f355a06a2dee70866e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571658"
---
# <a name="streamselectoperationgetresults-method"></a>Стреамселектоператион. results, метод

Возвращает результаты асинхронной операции, запущенной [**селектбестстреамасинк**](/previous-versions/windows/desktop/legacy/hh829001(v=vs.85)).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetResults(
  [out, retval] UINT32 *value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ out, retval\]
</dt> <dd></dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                          | Описание                      |
|--------------------------------------------------------------------------------------|----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl> | Метод выполнен успешно.<br/> |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**стреамселектоператион**](streamselectoperation.md)
</dt> </dl>

 

