---
description: Проверяет, может ли объект Инкдивидер использовать класс Инкрекогнизерконтекст для анализа слов.
ms.assetid: fd848fcc-5258-401f-8b51-b9d57da173da
title: Функция Рекогнизерконтекстсет
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- RecognizerContextSet
api_type:
- LibDef
api_location:
- InkDiv.dll
- InkDiv.dll.dll
ms.openlocfilehash: 51e75b810c2103afed2e8ac8a28706b9c9af5da0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459397"
---
# <a name="recognizercontextset-function"></a>Функция Рекогнизерконтекстсет

Проверяет, может ли объект [**инкдивидер**](inkdivider-class.md) использовать класс [**инкрекогнизерконтекст**](inkrecognizercontext-class.md) для анализа слов.

Эта функция не предназначена для использования в коде приложения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT WINAPI RecognizerContextSet(
  _In_ INT_PTR hDivider
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хдивидер* \[ окне\]
</dt> <dd>

Маркер объекта [**инкдивидер**](inkdivider-class.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция может возвращать одно из этих значений.



| Код возврата                                                                                  | Описание                                     |
|----------------------------------------------------------------------------------------------|-------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Функция выполнена успешно.<br/>              |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Недопустимый параметр *пдивидер* .<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                         |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                             |
| Библиотека<br/>                  | <dl> <dt>InkDiv.dll</dt> </dl> |



 

 




