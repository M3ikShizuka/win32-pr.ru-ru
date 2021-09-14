---
description: Вызывает вспомогательную функциональность для интерфейса IDispatch.
ms.assetid: ccef47af-d9dd-48c3-93d3-ee997dacf7a8
title: Функция Инвокеидиспатч
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- InvokeIDispatch
api_type:
- LibDef
api_location:
- InkObj.dll
- InkObj.dll.dll
ms.openlocfilehash: e4989e3ec23a1ffa97ba317831143ecf0920ef9b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460237"
---
# <a name="invokeidispatch-function"></a>Функция Инвокеидиспатч

Вызывает вспомогательную функциональность для интерфейса IDispatch.

Эта функция не предназначена для использования в коде приложения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT WINAPI InvokeIDispatch(
        IDispatch  *pDispatch,
        DISPID     dispid,
        DISPPARAMS *pDisp,
  _Out_ VARIANT    *pVarResult
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пдиспатч* 
</dt> <dd>

Экземпляр интерфейса IDispatch.

</dd> <dt>

*DISPID* 
</dt> <dd>

Метод, свойство или аргумент для передачи.

</dd> <dt>

*пдисп* 
</dt> <dd>

Параметры для передачи.

</dd> <dt>

*пварресулт* \[ заполняет\]
</dt> <dd>

Структура, принимающая извлеченные значения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается успешно, возвращается значение S \_ ОК. В случае неудачи возможные коды возврата включают, но не ограничиваются значениями, приведенными в следующей таблице.



| Код возврата                                                                                  | Описание                                      |
|----------------------------------------------------------------------------------------------|--------------------------------------------------|
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Недопустимое значение для *пдиспатч* .<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                         |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                             |
| Библиотека<br/>                  | <dl> <dt>InkObj.dll</dt> </dl> |



 

 




