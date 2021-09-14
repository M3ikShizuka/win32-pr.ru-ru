---
description: Возвращает уровень изоляции и значение времени ожидания транзакции, размещенной в корневом контексте транзакции.
ms.assetid: bb3ff03e-e69e-4a50-af36-4938eb4323df
title: 'Метод Иконтексттрансактионинфо:: Жеттксисолатионлевеландтимеаут'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextTransactionInfo.GetTxIsolationLevelAndTimeout
api_type:
- COM
api_location: ''
ms.openlocfilehash: b8545a697e672af7206a69ffa19618d5b70e055c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056144"
---
# <a name="icontexttransactioninfogettxisolationlevelandtimeout-method"></a>Метод Иконтексттрансактионинфо:: Жеттксисолатионлевеландтимеаут

Возвращает уровень изоляции и значение времени ожидания транзакции, размещенной в корневом контексте транзакции.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetTxIsolationLevelAndTimeout(
  [out] ISOLEVEL *pIsoLevel,
  [out] DWORD    *dwTime
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*писолевел* \[ заполняет\]
</dt> <dd>

Значение [ISOLATIONLEVEL](/previous-versions/windows/desktop/ms679234(v=vs.85)) для транзакции.

</dd> <dt>

*двтиме* \[ заполняет\]
</dt> <dd>

Время ожидания транзакции в секундах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать стандартные возвращаемые значения E \_ INVALIDARG, e \_ OUTOFMEMORY, e \_ непредвиденные и S \_ ОК.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 2 (SP2) \[ только классические приложения\]<br/>          |
| Минимальная версия сервера<br/> | Windows Только для настольных приложений сервера 2003 с пакетом обновления 1 \[\]<br/> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**иконтексттрансактионинфо**](icontexttransactioninfo.md)
</dt> </dl>

 

