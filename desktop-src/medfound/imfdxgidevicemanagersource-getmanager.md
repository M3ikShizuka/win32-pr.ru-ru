---
description: Возвращает Имфдксгидевицеманажер из приемника отрисовки Microsoft Media Foundation видео.
ms.assetid: 809e89e4-3ed5-4dba-82dc-4ec217b8ef38
title: 'Метод Имфдксгидевицеманажерсаурце:: Manage'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFDXGIDeviceManagerSource.GetManager
api_type:
- COM
api_location:
- mfidl.h
ms.openlocfilehash: 098810e9e06f339b1035748d71f46c7af26e96a8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462218"
---
# <a name="imfdxgidevicemanagersourcegetmanager-method"></a>Метод Имфдксгидевицеманажерсаурце:: Manage

Возвращает [**имфдксгидевицеманажер**](/windows/desktop/api/mfobjects/nn-mfobjects-imfdxgidevicemanager) из приемника отрисовки Microsoft Media Foundation видео.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetManager(
  [out] IMFDXGIDeviceManager **ppManager
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппманажер* \[ заполняет\]
</dt> <dd>

Объект [**имфдксгидевицеманажер**](/windows/desktop/api/mfobjects/nn-mfobjects-imfdxgidevicemanager) .

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

[**имфдксгидевицеманажерсаурце**](imfdxgidevicemanagersource.md)
</dt> </dl>

 

 




