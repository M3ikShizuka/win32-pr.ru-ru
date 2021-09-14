---
title: Метод использованием метода ibackgroundcopyjob Жетнотифифлагс (Deliveryoptimization. h)
description: Получает флаги уведомления о событии для задания.
ms.assetid: 95ADC97F-63DC-4EB6-B85C-7BCC79238C12
keywords:
- Метод Жетнотифифлагс
- Метод Жетнотифифлагс, интерфейс использованием метода ibackgroundcopyjob
- Интерфейс использованием метода ibackgroundcopyjob, метод Жетнотифифлагс
topic_type:
- apiref
api_name:
- IBackgroundCopyJob.GetNotifyFlags
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: e104857725849dfeb899b449ea055bc3cdb046bd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066444"
---
# <a name="ibackgroundcopyjobgetnotifyflags-method"></a>Метод использованием метода ibackgroundcopyjob:: Жетнотифифлагс

Получает флаги уведомления о событии для задания.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetNotifyFlags(
  [out] ULONG *pNotifyFlags
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пнотифифлагс* \[ заполняет\]
</dt> <dd>

Определяет события, получаемые приложением. В следующей таблице перечислены значения флагов уведомлений о событиях.



| Значение                                                                                                                                                                                                  | Значение                                                                        |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------|
| <span id="BG_NOTIFY_JOB_TRANSFERRED"></span><span id="bg_notify_job_transferred"></span><dl> <dt>**BG_NOTIFY_JOB_TRANSFERRED**</dt> </dl>    | Все файлы в задании были переданы.<br/>                  |
| <span id="BG_NOTIFY_JOB_ERROR"></span><span id="bg_notify_job_error"></span><dl> <dt>**BG_NOTIFY_JOB_ERROR**</dt> </dl>                      | Произошла ошибка.<br/>                                              |
| <span id="BG_NOTIFY_DISABLE"></span><span id="bg_notify_disable"></span><dl> <dt>**BG_NOTIFY_DISABLE**</dt> </dl>                             | Уведомление о событии отключено. Если этот параметр задан, другие флаги не учитываются.<br/> |
| <span id="BG_NOTIFY_JOB_MODIFICATION"></span><span id="bg_notify_job_modification"></span><dl> <dt>**BG_NOTIFY_JOB_MODIFICATION**</dt> </dl> | Задание было изменено.<br/>                                          |



 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения **HRESULT** , а также другие.



| Код возврата                                                                              | Описание                                                |
|------------------------------------------------------------------------------------------|------------------------------------------------------------|
| <dl> <dt>S_OK * * * *</dt> </dl> | Флаги уведомления о событии успешно получены.<br/> |



 

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

[**ибаккграундкопикаллбакк**](ibackgroundcopycallback.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: Жетнотифинтерфаце**](ibackgroundcopyjob-getnotifyinterface.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: Сетнотифифлагс**](ibackgroundcopyjob-setnotifyflags.md)
</dt> </dl>

 

 





