---
title: 'Метод IDeliveryOptimizationFile2:: SetProperty'
description: 'Этот метод возвращает одно свойство файла оптимизации доставки. | Метод IDeliveryOptimizationFile2:: SetProperty'
keywords:
- SetProperty — метод
- Метод SetProperty, интерфейс IDeliveryOptimizationFile2
- Интерфейс IDeliveryOptimizationFile2, метод SetProperty
topic_type:
- apiref
api_name:
- IDeliveryOptimizationFile2.SetProperty
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 01/18/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: c9c392c603ed067520b0f189dfbf547bc12ee80a
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520826"
---
# <a name="ideliveryoptimizationfile2setproperty-method"></a>Метод IDeliveryOptimizationFile2:: SetProperty

Этот метод возвращает одно свойство файла оптимизации доставки.

## <a name="syntax"></a>Синтаксис

```C++
HRESULT SetProperty(
  [in]               DOFilePropertyId propId,
  [in, unique] const VARIANT          *propValue
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*propId* \[ окне\]
</dt> <dd>

Обязательный идентификатор свойства для набора типа Дофилепропертид.

</dd> <dt>

*пропвалуе* \[ окне\]
</dt> <dd>

Заданное значение свойства типа VARIANT.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения HRESULT.

| Код возврата                  | Описание                                                        |
|------------------------------|--------------------------------------------------------------------|
| **S_OK**                     | Успешное завершение                                                            |
| **DO_E_UNKNOWN_PROPERTY_ID** | Неизвестный идентификатор свойства                                                |
| **DO_E_INVALID_STATE**       | Задание в настоящее время не находится в состоянии, допускающем установку свойства |

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

[**IDeliveryOptimizationFile2**](ideliveryoptimizationfile2.md)
