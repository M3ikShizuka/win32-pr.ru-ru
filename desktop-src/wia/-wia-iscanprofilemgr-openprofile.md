---
description: Открывает профиль сканирования, сохраненный на диске в виде XML-файла.
ms.assetid: 2b45280e-a1b6-4db9-af8c-09faff34b067
title: 'Метод Исканпрофилемгр:: Опенпрофиле (Сканпрофилемгр. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IScanProfileMgr.OpenProfile
api_type:
- COM
api_location:
- Scanprofilemgr.h
ms.openlocfilehash: 40d380a2b0405445cba72a0aac73c4b529114fcb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571399"
---
# <a name="iscanprofilemgropenprofile-method"></a>Метод Исканпрофилемгр:: Опенпрофиле

Открывает профиль сканирования, сохраненный на диске в виде XML-файла.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT OpenProfile(
  [in]  GUID         guid,
  [out] IScanProfile **ppScanProfile
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*идентификатор GUID* \[ окне\]
</dt> <dd>

Тип: **GUID**

Идентификатор GUID профиля.

</dd> <dt>

*ппсканпрофиле* \[ заполняет\]
</dt> <dd>

Тип: **[ **исканпрофиле**](-wia-iscanprofile.md)\*\***

Адрес указателя на профиль.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Если профиль сканирования сохранен с помощью метода [**Save**](-wia-iscanprofile-save.md) , он сохраняется в виде XML-файла в файле% UserProfile% \\ Application Data \\ \\ центра документов Microsoft \\ усерсканпрофилес.

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

 

 




