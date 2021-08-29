---
title: Метод GetType использованием метода ibackgroundcopyjob (Deliveryoptimization. h)
description: Возвращает тип выполняемой передачи, например скачивание файла или его отправку.
ms.assetid: F543A601-9385-4A73-A4E2-DE61433E84D3
keywords:
- GetType - метод
- Метод GetType, интерфейс использованием метода ibackgroundcopyjob
- Интерфейс использованием метода ibackgroundcopyjob, метод GetType
topic_type:
- apiref
api_name:
- IBackgroundCopyJob.GetType
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: e7697891e3ff98acd7440d52fe7be2799e4a551e45326c82a00d370e39fc4f1f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119755254"
---
# <a name="ibackgroundcopyjobgettype-method"></a>Метод использованием метода ibackgroundcopyjob:: GetType

Возвращает тип выполняемой передачи, например скачивание файла или его отправку.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetType(
  [out] BG_JOB_TYPE *pJobType
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пжобтипе* \[ заполняет\]
</dt> <dd>

Тип выполняемой операции перемещения. Список типов перемещения см. в разделе Перечисление [**BG_JOB_TYPE**](bg-job-type.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает следующие значения **HRESULT** , а также другие.



| Код возврата                                                                              | Описание                                          |
|------------------------------------------------------------------------------------------|------------------------------------------------------|
| <dl> <dt>S_OK * * * *</dt> </dl> | Тип перемещения успешно получен.<br/> |



 

## <a name="remarks"></a>Remarks

Укажите тип перемещения при создании задания.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>DeliveryOptimization. idl</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Досвк. lib</dt> </dl>                |
| DLL<br/>                      | <dl> <dt>Dosvc.dll</dt> </dl>                |
| IID<br/>                      | IID_IBackgroundCopyJob определен как 37668D37-507E-4160-9316-26306D150B12<br/>               |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Использованием метода ibackgroundcopyjob**](ibackgroundcopyjob-.md)
</dt> <dt>

[**BG_JOB_TYPE**](bg-job-type.md)
</dt> <dt>

[**Ибаккграундкопиманажер:: CreateJob**](ibackgroundcopymanager-createjob.md)
</dt> </dl>

 

 





