---
title: 'Идодовнлоад: метод:P Аусе'
description: Приостанавливает скачивание.
keywords:
- 'Идодовнлоад: метод:P Аусе'
topic_type:
- apiref
api_name:
- IDODownload.Pause
api_location:
- dosvc.dll
api_type:
- COM
ms.localizationpriority: low
ms.topic: reference
ms.date: 07/03/2019
ms.openlocfilehash: fd9598cb18790c78b32cddc04afb20e4a1a44efb111f2d562df2c6e1fe3f34fb
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119953634"
---
# <a name="idodownloadpause-method"></a>Идодовнлоад: метод:P Аусе

Приостанавливает скачивание.

## <a name="syntax"></a>Синтаксис

```cpp
HRESULT Pause();
```

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается с ошибкой, она возвращает **S_OK**. В противном случае возвращается [](/windows/desktop/com/structure-of-com-error-codes) [код ошибки](/windows/desktop/com/com-error-codes-10)HRESULT.

## <a name="requirements"></a>Requirements (Требования)

| &nbsp; | &nbsp; |
| ---- |:---- |
| **Минимальная версия клиента** | Windows 10, версия 1809 \[ Только приложения Win32\] |
| **Минимальная версия сервера** | Windows Сервер, \[ только приложения Win32 версии 1809\] |
| **Header** | Do. h |
