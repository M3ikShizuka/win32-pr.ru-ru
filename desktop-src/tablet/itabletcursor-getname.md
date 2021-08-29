---
description: Извлекает имя пера планшета.
ms.assetid: 94955c04-f699-428b-b4bf-53919b61b1ab
title: 'Метод Итаблеткурсор:: Name'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITabletCursor.GetName
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: 4fadbaa2fe170f04d40d46dffe8f16f0cb0fa3050baf30ea455972013c6d3e63
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118717313"
---
# <a name="itabletcursorgetname-method"></a>Метод Итаблеткурсор:: Name

Извлекает имя пера планшета.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetName(
  [out] LPWSTR *ppwszName
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппвсзнаме* \[ заполняет\]
</dt> <dd>

Имя пера планшета.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                            | Описание                               |
|----------------------------------------------------------------------------------------|-------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>   | Успешно.<br/>                       |
| <dl> <dt>**\_Ошибка E**</dt> </dl> | Произошла неизвестная ошибка.<br/> |



 

## <a name="remarks"></a>Remarks

Он отвечает за освобождение памяти, возвращаемой этим методом, с помощью [**CoTaskMemFree**](/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemfree).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Библиотека<br/>                  | <dl> <dt>Wisptis.exe</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**итаблеткурсор**](itabletcursor.md)
</dt> <dt>

[**Интерфейс Итаблеткурсорбуттон**](itabletcursorbutton.md)
</dt> </dl>

 

