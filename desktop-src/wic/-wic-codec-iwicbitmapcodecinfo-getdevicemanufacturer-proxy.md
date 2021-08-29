---
description: Функция-посредник для метода Жетдевицемануфактурер.
ms.assetid: f4dbf67a-eb67-4138-a77a-7386567b95e6
title: Функция IWICBitmapCodecInfo_GetDeviceManufacturer_Proxy
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWICBitmapCodecInfo_GetDeviceManufacturer_Proxy
api_type:
- DllExport
api_location:
- Windowscodecs.dll
- Wincodec.lib
ms.openlocfilehash: 0fe41dba0db5aa885817062a9fdc0300655b05f6a1e751c747e09af377076a54
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119812694"
---
# <a name="iwicbitmapcodecinfo_getdevicemanufacturer_proxy-function"></a>ИвикбитмапкодеЦинфо \_ жетдевицемануфактурер \_ -функция

Функция-посредник для метода [**жетдевицемануфактурер**](/windows/desktop/api/Wincodec/nf-wincodec-iwicbitmapcodecinfo-getdevicemanufacturer) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IWICBitmapCodecInfo_GetDeviceManufacturer_Proxy(
  _In_    IWICBitmapCodecInfo *THIS_PTR,
  _In_    UINT                cchDeviceManufacturer,
  _Inout_ WCHAR               *wzDeviceManufacturer,
  _Inout_ UINT                *pcchActual
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Этот \_* \[ Вход в\]
</dt> <dd>

Тип: **[ **ивикбитмапкодеЦинфо**](/windows/desktop/api/Wincodec/nn-wincodec-iwicbitmapcodecinfo)\***

Указатель на этот объект [**ивикбитмапкодеЦинфо**](/windows/desktop/api/Wincodec/nn-wincodec-iwicbitmapcodecinfo) .

</dd> <dt>

*кчдевицемануфактурер* \[ окне\]
</dt> <dd>

Тип: **uint**

Размер названия производства устройства.

</dd> <dt>

*вздевицемануфактурер* \[ в, out\]
</dt> <dd>

Тип: **WCHAR \***

Указатель, получающий имя производителя устройства.

</dd> <dt>

*пкчактуал* \[ в, out\]
</dt> <dd>

Тип: **uint \***

Фактический размер буфера, необходимый для получения имени производителя устройства.

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



 

 




