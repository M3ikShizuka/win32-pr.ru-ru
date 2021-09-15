---
description: Создает реализацию интерфейса Инкдивидер и возвращает его обработчик.
ms.assetid: 77c8504b-0b63-43dd-b487-bab2a500979b
title: Функция Креатеинкдивидер
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CreateInkDivider
api_type:
- LibDef
api_location:
- InkDiv.dll
- InkDiv.dll.dll
ms.openlocfilehash: 26e5785845f3ce8448269a821f67fcafc98bf4b3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344914"
---
# <a name="createinkdivider-function"></a>Функция Креатеинкдивидер

Создает реализацию интерфейса [**инкдивидер**](inkdivider-class.md) и возвращает его обработчик.

Эта функция не предназначена для использования в коде приложения.

## <a name="syntax"></a>Синтаксис


```C++
INT_PTR CreateInkDivider(void);
```



## <a name="parameters"></a>Параметры

У этой функции нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер для созданного объекта.

## <a name="remarks"></a>Комментарии

Этот класс наследуется от базового класса [**инкдивидер**](inkdivider-class.md) и реализует виртуальные функции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                         |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                             |
| Библиотека<br/>                  | <dl> <dt>InkDiv.dll</dt> </dl> |



 

 




