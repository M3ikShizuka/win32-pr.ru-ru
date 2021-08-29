---
description: Получает монопольную блокировку, если на данный момент она не удерживается другими.
ms.assetid: d655b89c-f2c8-4965-a21b-f539b1598296
title: 'Метод Кшарелоккнх:: Трексклусивелокк'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CShareLockNH.TryExclusiveLock
api_type:
- COM
api_location:
- Rwnh.dll
ms.openlocfilehash: 28bd569c287b00cf6b0a146022ade6ce7f7bf29d5ced9eb5ef62341c873059c6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119654664"
---
# <a name="csharelocknhtryexclusivelock-method"></a>Метод Кшарелоккнх:: Трексклусивелокк

Получает монопольную блокировку, если на данный момент она не удерживается другими.

## <a name="syntax"></a>Синтаксис


```C++
BOOL TryExclusiveLock();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если функция выполнена. в противном случае возвращается **значение false**.

## <a name="remarks"></a>Remarks

Эта функция не имеет связанной библиотеки импорта или файла заголовка. его необходимо вызвать с помощью функций [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) и [**GetProcAddress**](/windows/win32/api/libloaderapi/nf-libloaderapi-getprocaddress) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------|-------------------------------------------------------------------------------------|
| DLL<br/> | <dl> <dt>Rwnh.dll</dt> </dl> |



 

 
