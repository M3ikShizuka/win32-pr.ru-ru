---
title: Перечисление Деливерйоптимизатионфилепроперти (Deliveryoptimization. h)
description: Перечисление Деливерйоптимизатионфилепроперти указывает идентификатор необязательного свойства для файла оптимизации доставки.
keywords:
- Перечисление Деливерйоптимизатионфилепроперти
topic_type:
- apiref
api_name:
- DeliveryOptimizationFileProperty
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 01/18/2019
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 7c670118a66525c2a890a8c1ed96e4eefb5f5c28
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520256"
---
# <a name="deliveryoptimizationfileproperty-enumeration"></a>Перечисление Деливерйоптимизатионфилепроперти

Перечисление Деливерйоптимизатионфилепроперти указывает идентификатор необязательного свойства для файла оптимизации доставки. Это перечисление используется в интерфейсе IDeliveryOptimizationFile2, где передается значение свойства типа VARIANT.

## <a name="syntax"></a>Синтаксис

```C++
typedef enum _DeliveryOptimizationFileProperty {  
  DOFilePropertyId_DecryptionInfo,
  DOFilePropertyId_IntegrityCheckInfo,
  DOFilePropertyId_IntegrityCheckMandatory,
  DOFilePropertyId_DownloadSinkInterface,
  DOFilePropertyId_DownloadSinkFilePath,
  DOFilePropertyId_DownloadSinkMemoryStream,
  DOFilePropertyId_TotalSizeBytes
} DOFilePropertyId;
```

## <a name="constants"></a>Константы

<dl> <dt>

DOFilePropertyId_DecryptionInfo
</dt> <dd>

Идентификатор свойства DOFilePropertyId_DecryptionInfo задает сведения о расшифровке в виде строки JSON. DOFilePropertyId_DecryptionInfo является свойством только для записи типа VT_BSTR.

</dd> <dt>

DOFilePropertyId_IntegrityCheckInfo
</dt> <dd>

Идентификатор свойства DOFilePropertyId_IntegrityCheckInfo задает расположение файла хэш-кода (ФФ), которое используется оптимизацией доставки для выполнения проверок целостности во время выполнения для загруженного содержимого. DOFilePropertyId_IntegrityCheckInfo является свойством только для записи типа VT_BSTR.

</dd> <dt>

DOFilePropertyId_IntegrityCheckMandatory
</dt> <dd>

Идентификатор свойства DOFilePropertyId_IntegrityCheckMandatory задает логический флаг, указывающий, является ли использование ФФ обязательным. Если значение — TRUE, загрузка будет прервана после сбоя проверки целостности. DOFilePropertyId_IntegrityCheckMandatory является свойством для чтения и записи типа VT_BOOL.

</dd> <dt>

DOFilePropertyId_DownloadSinkFilePath
</dt> <dd>

Идентификатор свойства DOFilePropertyId_DownloadSinkFilePath задает полное расположение файловой системы, где оптимизация доставки должна хранить загруженные фрагменты. DOFilePropertyId_DownloadSinkFilePath имеет тип VT_BSTR.

</dd> <dt>

DOFilePropertyId_DownloadSinkMemoryStream
</dt> <dd>

Идентификатор свойства DOFilePropertyId_DownloadSinkMemoryStream является устаревшим. Не используйте.

</dd> <dt>

DOFilePropertyId_TotalSizeBytes
</dt> <dd>

Идентификатор свойства DOFilePropertyId_TotalSizeBytes указывает общий размер загрузки. DOFilePropertyId_TotalSizeBytes имеет тип VT_UI8.
</dd> </dl>

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------------------|----------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1803\]<br/>      |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>  |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl>               |
