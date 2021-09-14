---
title: Метод обратной передачи ИВМПДВД
description: Метод Back изменяет отображение из подменю на его родительское меню.
ms.assetid: 81d033d4-f570-44a5-898a-e419101c04fa
keywords:
- метод back проигрыватель Windows Media
- метод back проигрыватель Windows Media, интерфейс ивмпдвд
- интерфейс ивмпдвд проигрыватель Windows Media, метод back
topic_type:
- apiref
api_name:
- IWMPDVD.back
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4cd31cd6365843a6905760c4447ea679e15e70ed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242956"
---
# <a name="iwmpdvdback-method"></a>Метод ИВМПДВД:: Back

Метод **Back** изменяет отображение из подменю на его родительское меню.

## <a name="syntax"></a>Синтаксис


```CSharp
public void back();
```


```VB

Public Sub back()
Implements IWMPDVD.back
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Каждый DVD-диск создан по-другому. Некоторые DVD-диски созданы таким образом, чтобы `back` метод был доступен из корневого меню, но при его вызове ничего не делает.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс ИВМПДВД (VB и C#)**](iwmpdvd--vb-and-c.md)
</dt> </dl>

 

 





