---
title: Структура BG_FILE_RANGE (Deliveryoptimization. h)
description: Структура BG_FILE_RANGE определяет диапазон байтов для загрузки из файла.
ms.assetid: 58993C51-E42E-4E44-9E8A-15E982B25413
keywords:
- Структура BG_FILE_RANGE
topic_type:
- apiref
api_name:
- BG_FILE_RANGE
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 7d26785ba90ef6602ba7f5d0f4137d54e0b3044c
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128521171"
---
# <a name="bg_file_range-structure"></a>Структура BG_FILE_RANGE

Структура **BG_FILE_RANGE** определяет диапазон байтов для загрузки из файла.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  UINT64 InitialOffset;
  UINT64 Length;
} BG_FILE_RANGE;
```



## <a name="members"></a>Участники

<dl> <dt>

**инитиалоффсет**
</dt> <dd>

Смещение от нуля до начала диапазона байтов для скачивания из файла.

</dd> <dt>

**Длина**
</dt> <dd>

Длина диапазона в байтах. Не указывайте нулевую длину байта. Чтобы указать, что диапазон расширяется до конца файла, укажите **BG_LENGTH_TO_EOF**.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Диапазон должен существовать в файле или оптимизация доставки создает ошибку **DO_E_INVALID_RANGE** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IBackgroundCopyFile2:: Жетфилеранжес**](ibackgroundcopyfile2-getfileranges-method.md)
</dt> </dl>

 

 





