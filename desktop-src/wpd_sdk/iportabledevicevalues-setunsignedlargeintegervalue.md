---
description: Метод Сетунсигнедларжеинтежервалуе добавляет новое значение УЛОНГЛОНГ (тип VT \_ UI8) или перезаписывает существующий.
ms.assetid: 64874b86-7bf1-407a-8fff-a2c07c22f0cb
title: 'Метод Ипортабледевицевалуес:: Сетунсигнедларжеинтежервалуе (Портабледевицетипес. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPortableDeviceValues.SetUnsignedLargeIntegerValue
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
ms.openlocfilehash: 0c1ade76b4242c7508cb325e90c567349afcdc9d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458689"
---
# <a name="iportabledevicevaluessetunsignedlargeintegervalue-method"></a>Метод Ипортабледевицевалуес:: Сетунсигнедларжеинтежервалуе

Метод **сетунсигнедларжеинтежервалуе** добавляет новое значение **УЛОНГЛОНГ** (тип VT \_ UI8) или перезаписывает существующий.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetUnsignedLargeIntegerValue(
  [in]       REFPROPERTYKEY key,
  [in] const ULONGLONG      Value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ключ* \[ окне\]
</dt> <dd>

Объект **рефпропертикэй** , указывающий элемент для создания или перезаписи.

</dd> <dt>

*Значение* \[ окне\]
</dt> <dd>

Объект **улонглонг** , указывающий новое значение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                          | Описание                      |
|--------------------------------------------------------------------------------------|----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl> | Метод выполнен успешно.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Портабледевицетипес. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>Портабледевицегуидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Добавление ресурса в объект](adding-a-resource-to-an-object.md)
</dt> <dt>

[**Интерфейс Ипортабледевицевалуес**](iportabledevicevalues.md)
</dt> <dt>

[**Ипортабледевицевалуес:: Жетунсигнедларжеинтежервалуе**](iportabledevicevalues-getunsignedlargeintegervalue.md)
</dt> </dl>

 

 




