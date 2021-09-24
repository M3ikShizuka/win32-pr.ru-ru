---
title: 'Метод Идодовнлоадстатускаллбакк:: Онстатусчанже'
description: Оптимизация доставки вызывает реализацию этого метода при каждом изменении состояния загрузки.
keywords:
- 'Метод Идодовнлоадстатускаллбакк:: Онстатусчанже'
topic_type:
- apiref
api_name:
- IDODownloadStatusCallback.OnStatusChange
api_location:
- dosvc.dll
api_type:
- COM
ms.localizationpriority: low
ms.topic: reference
ms.date: 07/03/2019
ms.openlocfilehash: 6dcb30690736cb2bd2548fbd5f84cf580d317eff
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128519925"
---
# <a name="idodownloadstatuscallbackonstatuschange-method"></a>Метод Идодовнлоадстатускаллбакк:: Онстатусчанже

Оптимизация доставки вызывает реализацию этого метода при каждом изменении состояния загрузки.

## <a name="syntax"></a>Синтаксис

```cpp
HRESULT OnStatusChange(
  IDODownload *download,
  DO_DOWNLOAD_STATUS *status
);
```

## <a name="parameters"></a>Параметры

`download`

Указатель на интерфейс **идодовнлоад** , состояние которого изменилось.

`status`

Указатель на структуру **DO_DOWNLOAD_STATUS** , содержащую состояние загрузки.

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается с ошибкой, она возвращает **S_OK**. В противном случае возвращается [](/windows/desktop/com/structure-of-com-error-codes) [код ошибки](/windows/desktop/com/com-error-codes-10)HRESULT.

## <a name="requirements"></a>Требования

| &nbsp; | &nbsp; |
| ---- |:---- |
| **Минимальная версия клиента** | Windows 10, версия 1809 \[ Только приложения Win32\] |
| **Минимальная версия сервера** | Windows Сервер, \[ только приложения Win32 версии 1809\] |
| **Header** | Do. h |
