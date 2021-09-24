---
title: Метод использованием метода ibackgroundcopyjob Сетнопрогресстимеаут (Deliveryoptimization. h)
description: Задает период времени, в течение которого оптимизация доставки пытается переместить файл после возникновения временной ошибки. Если происходит выполнение, таймер сбрасывается.
ms.assetid: DC86F74F-8429-4D78-B425-CAF19867B05E
keywords:
- Метод Сетнопрогресстимеаут
- Метод Сетнопрогресстимеаут, интерфейс использованием метода ibackgroundcopyjob
- Интерфейс использованием метода ibackgroundcopyjob, метод Сетнопрогресстимеаут
topic_type:
- apiref
api_name:
- IBackgroundCopyJob.SetNoProgressTimeout
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 6e2bc77cf8a5c560cdc8a7bc7dd819c1dbe7a286
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520081"
---
# <a name="ibackgroundcopyjobsetnoprogresstimeout-method"></a>Метод использованием метода ibackgroundcopyjob:: Сетнопрогресстимеаут

Задает период времени, в течение которого оптимизация доставки пытается переместить файл после возникновения временной ошибки. Если происходит выполнение, таймер сбрасывается.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetNoProgressTimeout(
  [in] ULONG RetryPeriod
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Ретрипериод* \[ окне\]
</dt> <dd>

Время в секундах, в течение которого оптимизация доставки пытается переместить файл после того, как он не был выполнен. Период повтора по умолчанию для задания с высоким приоритетом составляет 3600 секунд (1 час), а для задания с низким приоритетом — 86400 секунд (24 часа).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения **HRESULT** , а также другие.



| Код возврата                                                                                          | Описание                                                                                          |
|------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| <dl> <dt>S_OK * * * *</dt> </dl>             | Период повтора успешно задан.<br/>                                                            |
| <dl> <dt>**DO_E_INVALID_STATE**</dt> </dl> | Состояние задания не может быть BG_JOB_STATE_CANCELLED или BG_JOB_STATE_ACKNOWLEDGED.<br/> |



 

## <a name="remarks"></a>Комментарии

Если оптимизация доставки не выполняется в течение периода повтора, она перемещает состояние задания с BG_JOB_STATE_TRANSIENT_ERROR на BG_JOB_STATE_ERROR. Если вы запрашиваете уведомление об ошибке, то оптимизация доставки вызывает обратный вызов [**жоберрор**](https://www.bing.com/search?q=**JobError**) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>DeliveryOptimization. idl</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Досвк. lib</dt> </dl>                |
| DLL<br/>                      | <dl> <dt>Dosvc.dll</dt> </dl>                |
| IID<br/>                      | IID_IBackgroundCopyJob определен как 37668D37-507E-4160-9316-26306D150B12<br/>               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Использованием метода ibackgroundcopyjob**](ibackgroundcopyjob-.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: Жетнопрогресстимеаут**](ibackgroundcopyjob-getnoprogresstimeout.md)
</dt> </dl>

 

 





