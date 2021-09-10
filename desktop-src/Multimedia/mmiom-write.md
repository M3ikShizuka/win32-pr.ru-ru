---
title: Сообщение MMIOM_WRITE (Ммсистем. h)
description: Сообщение ММИОМ \_ Write отправляется в процедуру ввода-вывода с помощью функции ммиоврите, чтобы запросить запись данных в открытый файл.
ms.assetid: 46e2dd9a-c4a7-4c99-86e4-a67b424411d1
keywords:
- сообщение MMIOM_WRITE Windows мультимедиа
topic_type:
- apiref
api_name:
- MMIOM_WRITE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c27cf96827f803608c369cc9022faa6235add9ec
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371121"
---
# <a name="mmiom_write-message"></a>\_Сообщение записи ммиом

Сообщение **ммиом \_ Write** отправляется в процедуру ввода-вывода с помощью функции [**ммиоврите**](/windows/win32/api/mmiscapi/nf-mmiscapi-mmiowrite) , чтобы запросить запись данных в открытый файл.


```C++
MMIOM_WRITE 
lParam1 = (LPARAM) lpBuffer 
lParam2 = (LPARAM) cbWrite 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lpBuffer"></span><span id="lpbuffer"></span><span id="LPBUFFER"></span>*лпбуффер*
</dt> <dd>

Указатель на буфер, содержащий данные для записи в файл.

</dd> <dt>

<span id="cbWrite"></span><span id="cbwrite"></span><span id="CBWRITE"></span>*кбврите*
</dt> <dd>

Число байтов для записи в файл.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает число байтов, фактически записанных в файл. Если возникает ошибка, возвращается значение 1.

## <a name="remarks"></a>Remarks

Процедура ввода-вывода отвечает за обновление элемента **лдискоффсет** структуры [**ммиоинфо**](/previous-versions//dd757322(v=vs.85)) для отражения нового расположения файла после операции записи.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



 

