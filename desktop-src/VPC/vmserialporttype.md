---
title: Перечисление Вмсериалпорттипе (Впккоминтерфацес. h)
description: Указывает тип последовательного порта.
ms.assetid: 1385292b-ee3c-41f0-805a-df126f33cabb
keywords:
- Перечисление Вмсериалпорттипе Virtual PC
topic_type:
- apiref
api_name:
- VMSerialPortType
api_location:
- VPCCOMInterfaces.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0733d09ddeadde0de93407be5d46661b536c6c9cebf0a96cec310aa2684b1509
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120124634"
---
# <a name="vmserialporttype-enumeration"></a>Перечисление Вмсериалпорттипе

\[Windows Virtual PC больше не доступен для использования в Windows 8. Вместо этого используйте [поставщик WMI Hyper-V (v2)](/windows/desktop/HyperV_v2/windows-virtualization-portal).\]

Указывает тип последовательного порта.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum  { 
  vmSerialPort_HostPort   = 0,
  vmSerialPort_TextFile   = 1,
  vmSerialPort_NamedPipe  = 2,
  vmSerialPort_Null       = 3
} VMSerialPortType;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="vmSerialPort_HostPort"></span><span id="vmserialport_hostport"></span><span id="VMSERIALPORT_HOSTPORT"></span>**Вмсериалпорт \_ хостпорт**
</dt> <dd>

Последовательный порт узла.

</dd> <dt>

<span id="vmSerialPort_TextFile"></span><span id="vmserialport_textfile"></span><span id="VMSERIALPORT_TEXTFILE"></span>**Вмсериалпорт \_ TextFile**
</dt> <dd>

Текстовый файл узла.

</dd> <dt>

<span id="vmSerialPort_NamedPipe"></span><span id="vmserialport_namedpipe"></span><span id="VMSERIALPORT_NAMEDPIPE"></span>**Вмсериалпорт \_ помощью канала NamedPipe**
</dt> <dd>

Именованный канал.

</dd> <dt>

<span id="vmSerialPort_Null"></span><span id="vmserialport_null"></span><span id="VMSERIALPORT_NULL"></span>**Вмсериалпорт \_ null**
</dt> <dd>

Последовательный порт, **равный null** (отклоняет все отправленные на него биты).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                    |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                     |
| Окончание поддержки клиента<br/>    | Windows 7<br/>                                                                          |
| Продукт<br/>                  | Windows Virtual PC<br/>                                                                 |
| Заголовок<br/>                   | <dl> <dt>Впккоминтерфацес. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ивмсериалпорт**](ivmserialport.md)
</dt> </dl>

 

