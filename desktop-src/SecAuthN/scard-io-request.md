---
description: '\_Структура запроса ввода-вывода бросить \_ начинает структуру данных управления протоколом.'
ms.assetid: 80fd7c6e-e768-42db-8302-29e92c9552f0
title: Структура SCARD_IO_REQUEST (Винсмкрд. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SCARD_IO_REQUEST
api_type:
- HeaderDef
api_location:
- Winsmcrd.h
ms.openlocfilehash: fe3205311789ee51bb9b96b3b425b735e1fdf887
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374976"
---
# <a name="scard_io_request-structure"></a>\_Структура запроса ввода-вывода бросить \_

Структура **\_ \_ запроса ввода-вывода бросить** начинает структуру данных управления протоколом. Все сведения, относящиеся к протоколу, затем следуют этой структуре сразу. Вся длина структуры должна быть согласована с базовым размером аппаратной архитектуры. Например, в Win32 длина любой информации PCI должна быть кратной четырем байтам, что соответствует 32-разрядной границе.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD dwProtocol;
  DWORD cbPciLength;
} SCARD_IO_REQUEST;
```



## <a name="members"></a>Участники

<dl> <dt>

**двпротокол**
</dt> <dd>

Используемый протокол.

</dd> <dt>

**кбпЦиленгс**
</dt> <dd>

Длина (в байтах) структуры **\_ \_ запроса ввода-вывода бросить** , а также следующие сведения, относящиеся к шине PCI.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Винсмкрд. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**SCardTransmit**](/windows/desktop/api/Winscard/nf-winscard-scardtransmit)
</dt> </dl>

 

 




