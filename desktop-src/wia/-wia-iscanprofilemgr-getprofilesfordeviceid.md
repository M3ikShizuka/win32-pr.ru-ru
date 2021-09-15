---
description: Возвращает все профили сканирования, связанные с устройством.
ms.assetid: 2e509f01-9c5e-4d17-8888-b08b6b4b9fa9
title: 'Метод Исканпрофилемгр:: Жетпрофилесфордевицеид (Сканпрофилемгр. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IScanProfileMgr.GetProfilesforDeviceID
api_type:
- COM
api_location:
- Scanprofilemgr.h
ms.openlocfilehash: 10a7d891a114fc36de3f91341febf1616a06ed22
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458785"
---
# <a name="iscanprofilemgrgetprofilesfordeviceid-method"></a>Метод Исканпрофилемгр:: Жетпрофилесфордевицеид

Возвращает все профили сканирования, связанные с устройством.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetProfilesforDeviceID(
  [in]      BSTR         bstrDeviceID,
  [in, out] ULONG        *pulNumProfiles,
  [out]     IScanProfile **ppScanProfile
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*бстрдевицеид* \[ окне\]
</dt> <dd>

Тип: **BSTR**

ИДЕНТИФИКАТОР устройства.

</dd> <dt>

*пулнумпрофилес* \[ в, out\]
</dt> <dd>

Тип: **ulong \***

При передаче указатель на максимальное число возвращаемых профилей. При возвращении возвращается указатель на число возвращаемых профилей.

</dd> <dt>

*ппсканпрофиле* \[ заполняет\]
</dt> <dd>

Тип: **[ **исканпрофиле**](-wia-iscanprofile.md)\*\***

Адрес указателя на массив профилей.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Если общее число профилей, связанных с устройством, меньше значения, переданного в *пулнумпрофилес*, то *пулнумпрофилес* возвращает этот итог. В противном случае возвращается то же значение, которое было передано в него.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                              |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                        |
| Заголовок<br/>                   | <dl> <dt>Сканпрофилемгр. h</dt> </dl> |
| IDL<br/>                      | <dl> <dt>Сканпрофилес. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**исканпрофилемгр**](-wia-iscanprofilemgr.md)
</dt> <dt>

[Схема профиля сканирования](-wia-scan-profile-schema.md)
</dt> </dl>

 

 




