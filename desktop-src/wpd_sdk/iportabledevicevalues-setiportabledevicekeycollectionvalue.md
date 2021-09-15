---
description: Метод Сетипортабледевицекэйколлектионвалуе добавляет новое значение Сетипортабледевицекэйколлектионвалуе (тип VT \_ Unknown) или перезаписывает существующий.
ms.assetid: f470cb89-e7a0-470d-83d1-eb643b062e45
title: 'Метод Ипортабледевицевалуес:: Сетипортабледевицекэйколлектионвалуе (Портабледевицетипес. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPortableDeviceValues.SetIPortableDeviceKeyCollectionValue
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
ms.openlocfilehash: face82230b9dd3bf6cbde18aaee8dd857e17d0a3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458704"
---
# <a name="iportabledevicevaluessetiportabledevicekeycollectionvalue-method"></a>Метод Ипортабледевицевалуес:: Сетипортабледевицекэйколлектионвалуе

Метод **сетипортабледевицекэйколлектионвалуе** добавляет новое значение **СЕТИПОРТАБЛЕДЕВИЦЕКЭЙКОЛЛЕКТИОНВАЛУЕ** (тип VT \_ Unknown) или перезаписывает существующий.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetIPortableDeviceKeyCollectionValue(
  [in] REFPROPERTYKEY               key,
  [in] IPortableDeviceKeyCollection *pValue
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ключ* \[ окне\]
</dt> <dd>

Объект **рефпропертикэй** , указывающий элемент для создания или перезаписи.

</dd> <dt>

*pValue* \[ окне\]
</dt> <dd>

Указатель на интерфейс **ипортабледевицекэйколлектион** , указывающий новое значение. Пакет SDK копирует ссылку на отправленный интерфейс и вызывает **AddRef** для него.

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

[**Ипортабледевицевалуес:: Жетипортабледевицекэйколлектионвалуе**](iportabledevicevalues-getiportabledevicekeycollectionvalue.md)
</dt> </dl>

 

 




