---
title: Метод использованием метода ibackgroundcopyjob Жетнотифинтерфаце (Deliveryoptimization. h)
description: Получает указатель интерфейса на реализацию интерфейса Ибаккграундкопикаллбакк.
ms.assetid: 1AA50C03-AC84-4AA9-8EC3-3FBA865C70C0
keywords:
- Метод Жетнотифинтерфаце
- Метод Жетнотифинтерфаце, интерфейс использованием метода ibackgroundcopyjob
- Интерфейс использованием метода ibackgroundcopyjob, метод Жетнотифинтерфаце
topic_type:
- apiref
api_name:
- IBackgroundCopyJob.GetNotifyInterface
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 6586a90de5783ceb24e5a7677f699a9cf6dfa60c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126970097"
---
# <a name="ibackgroundcopyjobgetnotifyinterface-method"></a>Метод использованием метода ibackgroundcopyjob:: Жетнотифинтерфаце

Получает указатель интерфейса на реализацию интерфейса [**ибаккграундкопикаллбакк**](ibackgroundcopycallback.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetNotifyInterface(
  [out] IUnknown **ppNotifyInterface
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппнотифинтерфаце* \[ заполняет\]
</dt> <dd>

Указатель интерфейса на реализацию интерфейса [**ибаккграундкопикаллбакк**](ibackgroundcopycallback.md) . По завершении выпустите *ппнотифинтерфаце*.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения **HRESULT** , а также другие.



| Код возврата                                                                              | Описание                                                           |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|
| <dl> <dt>S_OK * * * *</dt> </dl> | Указатель интерфейса уведомления успешно извлечен.<br/> |



 

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

[**Использованием метода ibackgroundcopyjob:: Жетнотифифлагс**](ibackgroundcopyjob-getnotifyflags.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: Сетнотифинтерфаце**](ibackgroundcopyjob-setnotifyinterface.md)
</dt> </dl>

 

 





