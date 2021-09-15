---
title: Ибасикдевице Уникуедевиценаме, метод
description: Извлекает уникальное имя устройства (УДН) устройства.
ms.assetid: 393EFF96-69E1-4081-905D-D8CC47B5FC4A
keywords:
- API потоковой передачи мультимедиа метода Уникуедевиценаме
- API потоковой передачи мультимедиа метода Уникуедевиценаме, интерфейс Ибасикдевице
- API потоковой передачи мультимедиа интерфейса Ибасикдевице, метод Уникуедевиценаме
topic_type:
- apiref
api_name:
- IBasicDevice.UniqueDeviceName
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 4b3103640fd49880dc5ae5ca881618ac1091de62
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460826"
---
# <a name="ibasicdeviceuniquedevicename-method"></a>Метод Ибасикдевице:: Уникуедевиценаме

Извлекает уникальное имя устройства (УДН) устройства.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT UniqueDeviceName(
  [out] HSTRING *value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ заполняет\]
</dt> <dd>

Получает указатель на УДН модель устройства.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает **значение HRESULT**. Допустимые значения включают, но не ограничиваются, значения, приведенные в следующей таблице.



| Код возврата                                                                          | Описание                      |
|--------------------------------------------------------------------------------------|----------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl> | Метод выполнен успешно.<br/> |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ибасикдевице**](ibasicdevice.md)
</dt> </dl>

 

 





