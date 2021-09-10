---
title: Команда сеттимекоде
description: Команда сеттимекоде включает или отключает запись времени в видеомагнитофоне. Устройства ВИДЕОМАГНИТОФОНА распознают эту команду.
ms.assetid: 1b4b82e8-4f13-4bc9-afb0-796339cabb51
keywords:
- команда сеттимекоде Windows мультимедиа
topic_type:
- apiref
api_name:
- settimecode
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 32092e5af7c77cdc274491b20663218d39a1ec1a
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370164"
---
# <a name="settimecode-command"></a>Команда сеттимекоде

Команда сеттимекоде включает или отключает запись времени в видеомагнитофоне. Устройства ВИДЕОМАГНИТОФОНА распознают эту команду.

Чтобы отправить эту команду, вызовите функцию [**mciSendString**](/previous-versions//dd757161(v=vs.85)) с заданным параметром *лпсзкомманд* , как показано ниже.

``` syntax
_stprintf_s(
  lpszCommand, 
  TEXT("settimecode %s %s %s"), 
  lpszDeviceID,
  lpszTimecode, 
  lpszFlags
); 
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lpszDeviceID"></span><span id="lpszdeviceid"></span><span id="LPSZDEVICEID"></span>*лпсздевицеид*
</dt> <dd>

Идентификатор устройства MCI. Этот идентификатор или псевдоним назначается при открытии устройства.

</dd> <dt>

<span id="lpszTimecode"></span><span id="lpsztimecode"></span><span id="LPSZTIMECODE"></span>*лпсзтимекоде*
</dt> <dd>

Один из следующих флагов.



| Значение      | Значение                          |
|------------|----------------------------------|
| запись в  | Задает запись времени в ВИДЕОМАГНИТОФОН. |
| запись отключена | Отключает запись времени.     |



 

</dd> <dt>

<span id="lpszFlags"></span><span id="lpszflags"></span><span id="LPSZFLAGS"></span>*лпсзфлагс*
</dt> <dd>

Может принимать значение "Wait", "notify", "Test" или их сочетание. Дополнительные сведения об этих флагах см. [в разделе Флаги ожидания, уведомления и проверки](the-wait-notify-and-test-flags.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>       |



## <a name="see-also"></a>См. также

<dl> <dt>

[MCI](mci.md)
</dt> <dt>

[Строки команд MCI](mci-command-strings.md)
</dt> </dl>

 

