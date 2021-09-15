---
description: останавливает режим приемника Miracast, отключает возможность обнаружения и отменяет регистрацию обратного вызова.
ms.assetid: 38AE60CB-F601-4C03-A725-9B802341B84B
title: Функция Вфддисплайсинкстоп (Вфдсинк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WFDStopDisplaySink
api_type:
- DllExport
api_location:
- wifidisplay.dll
ms.openlocfilehash: d1ebaa9920ca7d38cff22cef6383b37065faa2ba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461696"
---
# <a name="wfddisplaysinkstop-function"></a>Функция Вфддисплайсинкстоп

останавливает режим приемника Miracast, отключает возможность обнаружения и отменяет регистрацию обратного вызова. Приложение должно вызывать это после завершения работы.

## <a name="syntax"></a>Синтаксис


```C++
DWORD WINAPI WFDStopDisplaySink(void);
```



## <a name="parameters"></a>Параметры

У этой функции нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается успешно, возвращается значение ошибки \_ Success.

## <a name="remarks"></a>Remarks

Ожидается, что приложение разблокировало все выполняемые обратные вызовы перед вызовом **вфдстопдисплайсинк**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows 10<br/>                                                                      |
| Поддержка конца сервера<br/>    | Windows Server 2016<br/>                                                             |
| Заголовок<br/>                   | <dl> <dt>Вфдсинк. h</dt> </dl>       |
| Библиотека<br/>                  | <dl> <dt>Вифидисплай. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wifidisplay.dll</dt> </dl> |



 

 




