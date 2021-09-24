---
title: 'IDeliveryOptimizationJob2:: метод Property'
description: Возвращает одно свойство задания оптимизации доставки.
keywords:
- Метод GetProperty
- Метод Property, интерфейс IDeliveryOptimizationJob2
- Интерфейс IDeliveryOptimizationJob2, метод метода Property
topic_type:
- apiref
api_name:
- IDeliveryOptimizationJob2.GetProperty
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 01/18/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 2b849d4d9871a730e420f95b52f26b73b8e7b7a7
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520641"
---
# <a name="ideliveryoptimizationjob2getproperty-method"></a>IDeliveryOptimizationJob2:: метод Property

Этот метод возвращает одно свойство задания оптимизации доставки.

## <a name="syntax"></a>Синтаксис

```C++
HRESULT GetProperty(
  [in]  DOJobPropertyId propId,
  [out] VARIANT         *propValue
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*propId* \[ окне\]
</dt> <dd>

Требуемый идентификатор свойства для получения. Поддерживается только **DOJobPropertyId_ExtendedErrorInfo** типа VT_BSTR.

</dd> <dt>

*пропвалуе* \[ заполняет\]
</dt> <dd>

Результирующее значение свойства, хранящееся в типе VARIANT.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения HRESULT.

| Код возврата                  | Описание          |
|------------------------------|----------------------|
| **S_OK**                     | Успешное завершение              |
| **DO_E_UNKNOWN_PROPERTY_ID** | Неизвестный идентификатор свойства. |

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

## <a name="see-also"></a>См. также раздел

[**IDeliveryOptimizationJob2**](ideliveryoptimizationjob2.md)
