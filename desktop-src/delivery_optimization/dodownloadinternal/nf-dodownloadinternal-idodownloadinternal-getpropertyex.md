---
title: 'Метод Идодовнлоадинтернал:: Жетпропертекс'
description: Извлекает указатель на **вариант** , содержащий определенное значение расширенного свойства загрузки.
keywords:
- 'Метод Идодовнлоадинтернал:: Жетпропертекс'
topic_type:
- apiref
api_name:
- IDODownloadInternal.GetPropertyEx
api_location:
- dosvc.dll
api_type:
- COM
ms.localizationpriority: low
ms.topic: reference
ms.date: 07/29/2019
ms.openlocfilehash: 908f9b15df5c0c4a2769149419ff12d545201e5c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126965126"
---
# <a name="idodownloadinternalgetpropertyex-method"></a>Метод Идодовнлоадинтернал:: Жетпропертекс

> [!IMPORTANT]
> Интерфейс **идодовнлоадинтернал** является устаревшим. Вместо этого используйте интерфейс [идодовнлоад](../do/nn-do-idodownload.md) .

Извлекает указатель на **вариант** , содержащий определенное значение расширенного свойства загрузки.

## <a name="syntax"></a>Синтаксис

```cpp
HRESULT GetPropertyEx(
  DODownloadPropertyEx propId, 
  VARIANT* propVal
);
```

## <a name="parameters"></a>Параметры

`propId`

Обязательный идентификатор свойства для получения (типа **додовнлоадпропертекс**).

`propVal`

Результирующее значение свойства, хранящееся в **варианте**.

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается с ошибкой, она возвращает **S_OK**. В противном случае возвращается [](/windows/desktop/com/structure-of-com-error-codes) [код ошибки](/windows/desktop/com/com-error-codes-10)HRESULT.

|Возвращаемое значение|Описание|
|-|-|
|DO_E_UNKNOWN_PROPERTY_ID|*propId* неизвестен.|
|DO_E_WRITE_ONLY_PROPERTY|Свойство доступно только для записи и не может быть прочитано.|
|E_NOT_SET|Такое свойство не было задано через **сетпропертекс**.|

## <a name="requirements"></a>Требования

| &nbsp; | &nbsp; |
| ---- |:---- |
| **Минимальная версия клиента** | Windows 10, версия 1809 \[ Только приложения Win32\] |
| **Минимальная версия сервера** | Windows Сервер, \[ только приложения Win32 версии 1809\] |
| **Header** | Додовнлоадинтернал. h |