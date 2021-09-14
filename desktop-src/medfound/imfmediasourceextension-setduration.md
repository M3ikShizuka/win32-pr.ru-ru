---
description: Задает продолжительность источника мультимедиа в 100-наносекундных единицах.
ms.assetid: dc3dc600-ca81-40da-9edb-0af283ba9221
title: 'Метод Имфмедиасаурцеекстенсион:: Сетдуратион'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaSourceExtension.SetDuration
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: ae669bf19f531034eacafac7fb89f3c07fa1e0e9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462212"
---
# <a name="imfmediasourceextensionsetduration-method"></a>Метод Имфмедиасаурцеекстенсион:: Сетдуратион

Задает продолжительность источника мультимедиа в 100-наносекундных единицах.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetDuration(
  [in] double duration
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Длительность* \[ окне\]
</dt> <dd>

Длительность источника мультимедиа в единицах измерения 100-наносекундных.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                      |
| IDL<br/>                      | <dl> <dt>Мфмедиаенгине. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имфмедиасаурцеекстенсион**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediasourceextension)
</dt> </dl>

 

 




