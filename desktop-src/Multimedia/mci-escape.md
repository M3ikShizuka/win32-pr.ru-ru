---
title: Команда MCI_ESCAPE (Ммсистем. h)
description: '\_Управляющая команда MCI передает строку непосредственно на устройство. Устройства видеодиск распознают эту команду.'
ms.assetid: 56ebc717-f0f7-4612-8e51-57b13ff9d42b
keywords:
- команда MCI_ESCAPE Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_ESCAPE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 45a3c00955aa7476534f58c01f55e43d7cec562439741a9952372d19fda29a3a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119784529"
---
# <a name="mci_escape-command"></a>\_Управляющая команда MCI

\_Управляющая команда MCI передает строку непосредственно на устройство. Устройства видеодиск распознают эту команду.

Чтобы отправить эту команду, вызовите функцию [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) со следующими параметрами.


```C++
MCIERROR mciSendCommand(
  MCIDEVICEID wDeviceID, 
  MCI_ESCAPE, 
  DWORD dwFlags, 
  (DWORD) (LPMCI_VD_ESCAPE_PARMS) lpEscape
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="wDeviceID"></span><span id="wdeviceid"></span><span id="WDEVICEID"></span>*вдевицеид*
</dt> <dd>

Идентификатор устройства MCI, который должен получить командное сообщение.

</dd> <dt>

<span id="dwFlags"></span><span id="dwflags"></span><span id="DWFLAGS"></span>*dwFlags*
</dt> <dd>

\_Ожидание с уведомлением MCI или MCI \_ . Дополнительные сведения об этих флагах см. [в разделе Флаги ожидания, уведомления и проверки](the-wait-notify-and-test-flags.md).

</dd> <dt>

<span id="lpEscape"></span><span id="lpescape"></span><span id="LPESCAPE"></span>*лпескапе*
</dt> <dd>

Указатель на структуру [**\_ \_ \_ пармс ESC VD**](mci-vd-escape-parms.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

Данные, отправляемые с помощью управляющей клавиши MCI, \_ зависят от устройства и обычно передаются непосредственно на оборудование, связанное с устройством.

К устройствам видеодиск применяется следующий дополнительный флаг:

<dl> <dt>

<span id="MCI_VD_ESCAPE_STRING"></span><span id="mci_vd_escape_string"></span>\_Escape- \_ \_ строка VD MCI
</dt> <dd>

Командная строка указывается в элементе **лпстркомманд** структуры, определенной параметром *лпескапе*. Этот флаг является обязательным.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[MCI](mci.md)
</dt> <dt>

[Команды MCI](mci-commands.md)
</dt> </dl>

 

