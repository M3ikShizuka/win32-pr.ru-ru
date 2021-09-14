---
description: 'Метод Ипортабледевицевалуесколлектион:: RemoveAt — метод RemoveAt удаляет элемент, хранящийся в расположении, указанном заданным индексом.'
ms.assetid: 380212b6-5e71-406b-8236-e06672505f17
title: 'Метод Ипортабледевицевалуесколлектион:: RemoveAt (Портабледевицетипес. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPortableDeviceValuesCollection.RemoveAt
api_type:
- COM
api_location:
- PortableDeviceGUIDs.lib
- PortableDeviceGUIDs.dll
ms.openlocfilehash: 7db15480906bee8181bb0fc589c4f3e30ce4753c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127266872"
---
# <a name="iportabledevicevaluescollectionremoveat-method"></a>Метод Ипортабледевицевалуесколлектион:: RemoveAt

Метод **RemoveAt** удаляет элемент, хранящийся в расположении, заданном по заданному индексу.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT RemoveAt(
  [in] const DWORD dwIndex
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*двиндекс* \[ окне\]
</dt> <dd>

Указывает индекс удаляемого элемента.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                                  | Описание                                      |
|----------------------------------------------------------------------------------------------|--------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Метод выполнен успешно.<br/>                 |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Указанный индекс выходит за пределы допустимого диапазона.<br/> |



 

## <a name="remarks"></a>Remarks

Необходимо указать Отсчитываемый от нуля индекс.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Портабледевицетипес. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>Портабледевицегуидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ипортабледевицевалуесколлектион**](iportabledevicevaluescollection.md)
</dt> </dl>

 

 




