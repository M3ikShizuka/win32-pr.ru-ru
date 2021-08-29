---
title: 'Метод IDeliveryOptimizationJob2:: SetProperty'
description: Этот метод не используется.
keywords:
- SetProperty — метод
- Метод SetProperty, интерфейс IDeliveryOptimizationJob2
- Интерфейс IDeliveryOptimizationJob2, метод SetProperty
topic_type:
- apiref
api_name:
- IDeliveryOptimizationJob2.SetProperty
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 01/18/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 8495b51f8e799cb2e05a65aae143207d07489bac050569258d4b3218ad1f807e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118811155"
---
# <a name="ideliveryoptimizationjob2setproperty-method"></a>Метод IDeliveryOptimizationJob2:: SetProperty

Этот метод не используется.

## <a name="syntax"></a>Синтаксис

```C++
HRESULT SetProperty(
  [in]               DOJobPropertyId propId,
  [in, unique] const VARIANT         *propValue
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*propId* \[ окне\]
</dt> <dd>

Не используется.

</dd> <dt>

*пропвалуе* \[ окне\]
</dt> <dd>

Не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если propId имеет **DOJobPropertyId_ExtendedErrorInfo**, возвращаемое значение равно **DO_E_READ_ONLY_PROPERTY**, в противном случае функция возвращает **DO_E_UNKNOWN_PROPERTY_ID**.

## <a name="requirements"></a>Требования

| Требование | Значение |
|---------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента  | Windows 10, только для \[ настольных приложений версии 1803\]                                   |
| Минимальная версия сервера  | Windows Server, только для \[ настольных приложений версии 1709\]                               |
| Заголовок                    | Deliveryoptimization. h                                                           |
| IDL                       | DeliveryOptimization. idl                                                         |
| Библиотека                   | Досвк. lib                                                                        |
| DLL                       | Dosvc.dll                                                                        |
| IID                       | IID_IDeliveryOptimizationJob2 определен как 18995A26-BF59-4ABE-9F8B-D5092D5A2405 |

## <a name="see-also"></a>См. также

[**IDeliveryOptimizationJob2**](ideliveryoptimizationjob2.md)
