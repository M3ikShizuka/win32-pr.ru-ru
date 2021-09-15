---
description: Задает образец для источника потока мультимедиа.
ms.assetid: a35c5e18-f307-4e40-bc92-f91aa9eb80ba
title: 'Метод Имфмедиастреамсаурцесамплерекуест:: Сетсампле'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaStreamSourceSampleRequest.SetSample
api_type:
- COM
api_location:
- mfidl.h
ms.openlocfilehash: bc3b2693a4690207f0b39d7f1b846e1e63069a8c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462210"
---
# <a name="imfmediastreamsourcesamplerequestsetsample-method"></a>Метод Имфмедиастреамсаурцесамплерекуест:: Сетсампле

Задает образец для источника потока мультимедиа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetSample(
  [in] IMFSample *value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ окне\]
</dt> <dd>

Образец для источника потока мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ приложения UWP для классических приложений \|\]<br/>                                  |
| Минимальная версия сервера<br/> | Windows Server 2012 Приложения универсального \[ приложения UWP для настольных приложений \|\]<br/>                       |
| IDL<br/>                      | <dl> <dt>Мфидл. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имфмедиастреамсаурцесамплерекуест**](imfmediastreamsourcesamplerequest.md)
</dt> </dl>

 

 




