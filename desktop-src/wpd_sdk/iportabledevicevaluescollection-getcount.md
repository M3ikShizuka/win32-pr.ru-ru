---
description: 'Метод Ипортабледевицевалуесколлектион:: NOCOUNT — метод NOCOUNT извлекает количество элементов в коллекции.'
ms.assetid: c7b80a54-9e74-42d9-9155-cfcb2a92d324
title: 'Метод Ипортабледевицевалуесколлектион:: NOCOUNT (Портабледевицетипес. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPortableDeviceValuesCollection.GetCount
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
ms.openlocfilehash: 8304184f3323feb92a14b523dc629c6ae45f6a85
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571207"
---
# <a name="iportabledevicevaluescollectiongetcount-method"></a>Метод Ипортабледевицевалуесколлектион:: NOCOUNT

Метод **NOCOUNT** извлекает количество элементов в коллекции.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetCount(
  [in] DWORD *pcElems
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пцелемс* \[ окне\]
</dt> <dd>

Указатель на **DWORD** , содержащий число интерфейсов **ипортабледевицевалуес** в коллекции.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                               | Описание                                          |
|-------------------------------------------------------------------------------------------|------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>      | Метод выполнен успешно.<br/>                     |
| <dl> <dt>**\_указатель E**</dt> </dl> | Обязательный аргумент-указатель имеет **значение NULL**.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Портабледевицетипес. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>Портабледевицегуидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ипортабледевицевалуесколлектион**](iportabledevicevaluescollection.md)
</dt> </dl>

 

 




