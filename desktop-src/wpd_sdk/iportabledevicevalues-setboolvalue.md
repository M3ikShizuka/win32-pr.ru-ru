---
description: Метод SetBoolValue добавляет новое логическое значение (тип VT \_ bool) или перезаписывает существующий.
ms.assetid: add30665-78f7-4037-801e-af51a4ab2f60
title: 'Метод Ипортабледевицевалуес:: SetBoolValue (Портабледевицетипес. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPortableDeviceValues.SetBoolValue
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
ms.openlocfilehash: 7adf311e863c08873aa8300f9e940d4a5b49417f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570134"
---
# <a name="iportabledevicevaluessetboolvalue-method"></a>Метод Ипортабледевицевалуес:: SetBoolValue

Метод **SetBoolValue** добавляет новое **логическое** значение (тип VT \_ bool) или перезаписывает существующий.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetBoolValue(
  [in]       REFPROPERTYKEY key,
  [in] const BOOL           Value
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

**Bool** , указывающий новое значение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                          | Описание                      |
|--------------------------------------------------------------------------------------|----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl> | Метод выполнен успешно.<br/> |



 

## <a name="remarks"></a>Remarks

Если существующее значение имеет тот же ключ, что и параметр *Key* , он перезаписывает существующее значение без предупреждения. Существующий ключ памяти освобождается соответствующим образом.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Портабледевицетипес. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>Портабледевицегуидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ипортабледевицевалуес**](iportabledevicevalues.md)
</dt> <dt>

[**Ипортабледевицевалуес:: Жетбулвалуе**](iportabledevicevalues-getboolvalue.md)
</dt> </dl>

 

 




