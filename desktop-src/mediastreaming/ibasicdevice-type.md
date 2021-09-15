---
title: Метод типа Ибасикдевице
description: Возвращает значение перечисления, указывающее тип устройства DLNA.
ms.assetid: D9FB3A02-7796-4ACB-B7D3-D171D1D9B77F
keywords:
- Метод типа потоковая передача мультимедиа API
- Метод Type потоковая передача мультимедиа API, интерфейс Ибасикдевице
- API потоковой передачи мультимедиа интерфейса Ибасикдевице, метод Type
topic_type:
- apiref
api_name:
- IBasicDevice.Type
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a69f0671c82363ff61179c0120b3db8f6e755de9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460827"
---
# <a name="ibasicdevicetype-method"></a>Метод Ибасикдевице:: Type

Возвращает значение перечисления, указывающее тип устройства DLNA.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Type(
  [out] DeviceTypes *value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ заполняет\]
</dt> <dd>

Получает указатель на значение [**девицетипес**](devicetypes.md) .

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

 

 





