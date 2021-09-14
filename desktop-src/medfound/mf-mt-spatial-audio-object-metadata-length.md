---
description: Значение, указывающее размер (в байтах) типа объекта метаданных пространственного аудио, который будет выводиться декодером.
ms.assetid: C133693D-A8D5-4520-B561-57BF11074257
title: Атрибут MF_MT_SPATIAL_AUDIO_OBJECT_METADATA_LENGTH (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a2cd0b3cab788dbc724ab896d2cbfeb0d42f633f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363949"
---
# <a name="mf_mt_spatial_audio_object_metadata_length-attribute"></a>\_ \_ \_ \_ \_ Атрибут длины метаданных объекта пространственного звука \_ MF MT

Значение, указывающее размер (в байтах) типа объекта метаданных пространственного аудио, который будет выводиться декодером.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Большой двоичный объект метаданных с указанным форматом записывается с помощью интерфейса [**испатиалаудиометадатавритер**](/windows/win32/api/spatialaudiometadata/nn-spatialaudiometadata-ispatialaudiometadatawriter) и считывается с помощью интерфейса [**испатиалаудиометадатареадер**](/windows/win32/api/spatialaudiometadata/nn-spatialaudiometadata-ispatialaudiometadatareader) . Большой двоичный объект метаданных непрозрачен для Media Foundation конвейера и компонентов. Атрибут применяется к типу пространственного звукового носителя.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1703\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Мфапи. h</dt> </dl> |



 

 
