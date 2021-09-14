---
title: Метод использованием метода ibackgroundcopyjob-предыдущих версий (Deliveryoptimization. h)
description: Возвращает уровень приоритета для задания. Уровень приоритета определяет, когда задание обрабатывается относительно других заданий в очереди обмена.
ms.assetid: 2F778B35-8DBB-4540-88C2-A2E18EBB0D89
keywords:
- Метод предшествовал
- Метод использованием метода ibackgroundcopyjob, интерфейс
- Интерфейс использованием метода ibackgroundcopyjob, метод предшествовал
topic_type:
- apiref
api_name:
- IBackgroundCopyJob.GetPriority
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 7ae9a865045ee1264a0598a3d3c1db8cc3c3b8bc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056100"
---
# <a name="ibackgroundcopyjobgetpriority-method"></a>Метод использованием метода ibackgroundcopyjob:: предшествовал

Возвращает уровень приоритета для задания. Уровень приоритета определяет, когда задание обрабатывается относительно других заданий в очереди обмена.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetPriority(
  [out] BG_JOB_PRIORITY *pPriority
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пприорити* \[ заполняет\]
</dt> <dd>

Приоритет задания относительно других заданий в очереди обмена.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения **HRESULT** , а также другие.



| Код возврата                                                                              | Описание                                           |
|------------------------------------------------------------------------------------------|-------------------------------------------------------|
| <dl> <dt>S_OK * * * *</dt> </dl> | Уровень приоритета успешно получен.<br/> |



 

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



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Использованием метода ibackgroundcopyjob**](ibackgroundcopyjob-.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: SetPriority**](ibackgroundcopyjob-setpriority.md)
</dt> </dl>

 

 





