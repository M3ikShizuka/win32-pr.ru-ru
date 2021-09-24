---
title: Структура BG_JOB_PROGRESS (Deliveryoptimization. h)
description: Структура BG_JOB_PROGRESS предоставляет сведения о ходе выполнения, связанные с заданиями, такие как число переданных байтов и файлов. Для заданий отправки это состояние применяется к файлу отправки, а не к файлу ответов.
ms.assetid: F07BBDDE-FD34-4779-9E17-3789A8098616
keywords:
- Структура BG_JOB_PROGRESS
topic_type:
- apiref
api_name:
- BG_JOB_PROGRESS
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: f948b9b1150550fad432b0b816f8d435f2af0b4d
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128521181"
---
# <a name="bg_job_progress-structure"></a>Структура BG_JOB_PROGRESS

Структура **BG_JOB_PROGRESS** предоставляет сведения о ходе выполнения, связанные с заданиями, такие как число переданных байтов и файлов. Для заданий отправки это состояние применяется к файлу отправки, а не к файлу ответов.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _BG_JOB_PROGRESS {
  UINT64 BytesTotal;
  UINT64 BytesTransferred;
  ULONG  FilesTotal;
  ULONG  FilesTransferred;
} BG_JOB_PROGRESS;
```



## <a name="members"></a>Участники

<dl> <dt>

**BytesTotal**
</dt> <dd>

Общее число байтов для пересылки для всех файлов в задании. Если значение равно BG_SIZE_UNKNOWN, общий размер всех файлов в задании не определен. Оптимизация доставки не устанавливает это значение, если не может определить размер одного из файлов. Например, если указанный файл или сервер не существует, то оптимизация доставки не сможет определить размер файла.

При скачивании диапазонов из файла **битестотал** включает в себя общее число байтов, которое необходимо скачать из файла.

</dd> <dt>

**BytesTransferred**
</dt> <dd>

Число переданных байтов.

</dd> <dt>

**филестотал**
</dt> <dd>

Общее число переносимых файлов для этого задания.

</dd> <dt>

**филестрансферред**
</dt> <dd>

Число переданных файлов.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**BG_FILE_PROGRESS**](bg-file-progress.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: Progress**](ibackgroundcopyjob-getprogress.md)
</dt> </dl>

 

 





