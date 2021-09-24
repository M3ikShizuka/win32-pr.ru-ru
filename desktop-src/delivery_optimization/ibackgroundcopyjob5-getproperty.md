---
title: Метод IBackgroundCopyJob5-Property (Deliveryoptimization. h)
description: Универсальный метод для получения свойств задания оптимизации доставки.
ms.assetid: 22BA2FAB-3F24-4801-8FB7-CB6F9E8DFBB3
keywords:
- Метод GetProperty
- Метод Property, интерфейс IBackgroundCopyJob5
- Интерфейс IBackgroundCopyJob5, метод метода Property
topic_type:
- apiref
api_name:
- IBackgroundCopyJob5.GetProperty
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 6c09d5886acb7d1bada165180e3d26bdf6505a6b
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520276"
---
# <a name="ibackgroundcopyjob5getproperty-method"></a>IBackgroundCopyJob5:: метод Property

Универсальный метод для получения свойств задания оптимизации доставки.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetProperty(
  [in]  BITS_JOB_PROPERTY_ID    PropertyId,
  [out] BITS_JOB_PROPERTY_VALUE *pPropertyValue
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*PropertyId* \[ окне\]
</dt> <dd>

Идентификатор свойства, которое получается в виде значения перечисления [**BITS_JOB_PROPERTY_ID**](bits-job-property-id.md) .

</dd> <dt>

*ппропертивалуе* \[ заполняет\]
</dt> <dd>

Значение свойства, возвращаемое в виде BITS_JOB_PROPERTY_VALUE объединения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает следующие возвращаемые значения.



| Код возврата                                                                          | Описание        |
|--------------------------------------------------------------------------------------|--------------------|
| <dl> <dt>**S_OK**</dt> </dl> | Успешное завершение<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>DeliveryOptimization. idl</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Досвк. lib</dt> </dl>                |
| DLL<br/>                      | <dl> <dt>Dosvc.dll</dt> </dl>                |
| IID<br/>                      | IID_IBackgroundCopyJob5 определяется как E847030C-БББА-4657-AF6D-484AA42BF1FE<br/>              |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IBackgroundCopyJob5**](ibackgroundcopyjob5.md)
</dt> <dt>

[**IBackgroundCopyJob5:: SetProperty**](ibackgroundcopyjob5-setproperty.md)
</dt> </dl>

 

 





