---
title: Сообщение MM_MIM_LONGDATA (Ммсистем. h)
description: сообщение MM \_ MIM \_ лонгдата отправляется в окно, когда получено сообщение об истечении времени получения из системы MIDI или если буфер заполнен данными, исключающий систему.
ms.assetid: 72b9eade-4224-436f-bfef-32204eaf51ae
keywords:
- сообщение MM_MIM_LONGDATA Windows мультимедиа
topic_type:
- apiref
api_name:
- MM_MIM_LONGDATA
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 25bf1900ef2e9394b9d8772747eba873f8d607f1
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370902"
---
# <a name="mm_mim_longdata-message"></a>MM \_ MIM \_ сообщение лонгдата

сообщение **MM \_ MIM \_ лонгдата** отправляется в окно, когда получено сообщение об истечении времени получения из системы MIDI или если буфер заполнен данными, исключающий систему.


```C++
MM_MIM_LONGDATA 
wParam = (WPARAM) hInput 
lParam = (LPARAM) lpMidiHdr 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hInput"></span><span id="hinput"></span><span id="HINPUT"></span>*хинпут*
</dt> <dd>

Обработчик для входного устройства MIDI, получившего данные.

</dd> <dt>

<span id="lpMidiHdr"></span><span id="lpmidihdr"></span><span id="LPMIDIHDR"></span>*лпмидихдр*
</dt> <dd>

Указатель на структуру [**мидихдр**](/windows/win32/api/mmeapi/ns-mmeapi-midihdr) , определяющую буфер.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не возвращает значение.

## <a name="remarks"></a>Remarks

Возвращенный буфер может быть незаполненным. Чтобы определить число байтов, записанных в возвращенный буфер, используйте элемент **двбитесрекордед** структуры [**мидихдр**](/windows/win32/api/mmeapi/ns-mmeapi-midihdr) , на который указывает *лпмидихдр*.

Нет отметки времени, доступной для этого сообщения. Для входных данных с отметкой времени необходимо использовать сообщения, отправленные в функции обратного вызова.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Цифровой интерфейс музыкальных инструментов (MIDI)](musical-instrument-digital-interface--midi.md)
</dt> <dt>

[Сообщения MIDI](midi-messages.md)
</dt> </dl>

 

