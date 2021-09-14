---
title: Функция Утилстрингкопивисаллок (Ндаттрибутилс. h)
description: Выделяет и копирует исходную строку.
ms.assetid: e1400ae1-0edd-4b59-af03-3da1b9d7073b
keywords:
- Утилстрингкопивисаллок функция NDF
topic_type:
- apiref
api_name:
- UtilStringCopyWithAlloc
api_location:
- ndattributils.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b68bd1815ff09473f0431dde19a12a87603a9dec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065089"
---
# <a name="utilstringcopywithalloc-function"></a>Функция Утилстрингкопивисаллок

Функция **утилстрингкопивисаллок** выделяет и копирует исходную строку.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT UtilStringCopyWithAlloc(
  _Out_ LPWSTR  *Buffer,
  _In_  UINT    BufferMax,
  _In_  LPCWSTR Source
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Буфер* \[ заполняет\]
</dt> <dd>

Тип: **LPWSTR \***

Расположение, в котором хранится указатель на выделенную память. Если он больше не нужен, он должен быть выпущен с помощью [**CoTaskMemFree**](/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemfree). Этот буфер всегда завершается нулем.

</dd> <dt>

*Буффермакс* \[ окне\]
</dt> <dd>

Тип: **uint**

Максимальное число символов для чтения из *источника*.

</dd> <dt>

*Исходный код* \[ окне\]
</dt> <dd>

Тип: **лпквстр**

Копируемая строка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Возможные возвращаемые значения включают, но не ограничиваются следующим.



| Код возврата                                                                                  | Описание                                                        |
|----------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Операция успешно выполнена.<br/>                                |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Один или несколько параметров указаны неправильно.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Ндаттрибутилс. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**CoTaskMemFree**](/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemfree)
</dt> <dt>

[**утилассемблестрингсвисаллок**](utilassemblestringswithalloc.md)
</dt> <dt>

[**утиллоадстрингвисаллок**](utilloadstringwithalloc.md)
</dt> </dl>

 

