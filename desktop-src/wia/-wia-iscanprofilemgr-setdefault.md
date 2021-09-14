---
description: Задает указанный профиль сканирования в качестве профиля по умолчанию.
ms.assetid: c680be8b-88f0-4f7f-b1a3-e12711dba870
title: 'Метод Исканпрофилемгр:: Сетдефаулт (Сканпрофилемгр. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IScanProfileMgr.SetDefault
api_type:
- COM
api_location:
- Scanprofilemgr.h
ms.openlocfilehash: 3a7c32f246bcafc8ff7ce55e8c6f34ea45553a95
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127251824"
---
# <a name="iscanprofilemgrsetdefault-method"></a>Метод Исканпрофилемгр:: Сетдефаулт

Задает указанный профиль сканирования в качестве профиля по умолчанию.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetDefault(
  [in] IScanProfile *pScanProfile
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*псканпрофиле* \[ окне\]
</dt> <dd>

Тип: **[ **исканпрофиле**](-wia-iscanprofile.md)\***

Указатель на профиль.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Используйте метод **исканпрофилемгр:: сетдефаулт** , чтобы добавить `<Default>` элемент в профиль или удалить этот элемент из предыдущего профиля по умолчанию устройства.

Используйте метод [**сканпрофиледиалог**](-wia-iscanprofileui-scanprofiledialog.md) для изменения профиля по умолчанию.

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

 

 




