---
title: Функция Копихелператтрибуте (Ндаттрибутилс. h)
description: Создает копию структуры ВСПОМОГАТЕЛЬного \_ атрибута.
ms.assetid: ff49be29-4cd8-4730-929f-c66a7325704f
keywords:
- Копихелператтрибуте функция NDF
topic_type:
- apiref
api_name:
- CopyHelperAttribute
api_location:
- ndattributils.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 59fac3449ee48659980681c836d24406c4db7e2b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147110"
---
# <a name="copyhelperattribute-function"></a>Функция Копихелператтрибуте

Функция **копихелператтрибуте** создает копию структуры [**вспомогательного \_ атрибута**](/windows/win32/api/ndattrib/ns-ndattrib-helper_attribute) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CopyHelperAttribute(
  _Out_       HELPER_ATTRIBUTE *Dest,
  _In_  const HELPER_ATTRIBUTE *Source
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Конечный адрес* \[ заполняет\]
</dt> <dd>

Тип: **[ **вспомогательный \_ атрибут**](/windows/win32/api/ndattrib/ns-ndattrib-helper_attribute)\***

Обновляемая структура.

</dd> <dt>

*Исходный код* \[ окне\]
</dt> <dd>

Тип: **\* [**\_ атрибут вспомогательной**](/windows/win32/api/ndattrib/ns-ndattrib-helper_attribute) функции const**

Существующая копируемая структура.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Возможные возвращаемые значения включают, но не ограничиваются следующим.



| Код возврата                                                                                   | Описание                                                                 |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>          | Операция успешно выполнена.<br/>                                         |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl>  | Один или несколько параметров указаны неправильно.<br/>          |
| <dl> <dt>**E \_ OUTOFMEMORY**</dt> </dl> | Недостаточно памяти для выполнения этой операции.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Ндаттрибутилс. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ВСПОМОГАТЕЛЬный \_ атрибут**](/windows/win32/api/ndattrib/ns-ndattrib-helper_attribute)
</dt> </dl>

 

 





