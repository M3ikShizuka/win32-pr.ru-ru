---
description: Функция-посредник для метода Жетчаннелкаунт.
ms.assetid: f74916d9-d4b5-4b1b-adba-489d46c8d81c
title: Функция IWICPixelFormatInfo_GetChannelCount_Proxy
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWICPixelFormatInfo_GetChannelCount_Proxy
api_type:
- DllExport
api_location:
- Windowscodecs.dll
- Wincodec.lib
ms.openlocfilehash: eaaf0abc2c32e7a5a4469a3959875e28bb29d840f9da43f9bbbcc88fe56df788
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119812124"
---
# <a name="iwicpixelformatinfo_getchannelcount_proxy-function"></a>Ивикпикселформатинфо \_ жетчаннелкаунт \_ -функция

Функция-посредник для метода [**жетчаннелкаунт**](/windows/desktop/api/Wincodec/nf-wincodec-iwicpixelformatinfo-getchannelcount) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IWICPixelFormatInfo_GetChannelCount_Proxy(
  _In_  IWICPixelFormatInfo *THIS_PTR,
  _Out_ UINT                *puiChannelCount
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Этот \_* \[ Вход в\]
</dt> <dd>

Тип: **[ **ивикпикселформатинфо**](/windows/desktop/api/Wincodec/nn-wincodec-iwicpixelformatinfo)\***

Указатель на этот объект [**ивикпикселформатинфо**](/windows/desktop/api/Wincodec/nn-wincodec-iwicpixelformatinfo) .

</dd> <dt>

*пуичаннелкаунт* \[ заполняет\]
</dt> <dd>

Тип: **uint \***

Указатель, получающий число каналов.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если эта функция завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 2 (SP2), Windows \[ только классические приложения Vista\]<br/>                                                                                              |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                                                                             |
| DLL<br/>                      | <dl> <dt>Windowscodecs.dll; </dt> <dt>Винкодек. lib</dt> </dl> |



 

 




