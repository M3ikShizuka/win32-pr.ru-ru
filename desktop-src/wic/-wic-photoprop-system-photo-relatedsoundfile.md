---
description: Политика метаданных фотографии для свойства System. photo. Релатедсаундфиле.
ms.assetid: 3b212d90-7ae2-4b7c-b77a-2017490aca40
title: Политика метаданных фото для System. photo. Релатедсаундфиле
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 07a29adb71f572868f21b1b8427e71b09616b24c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247531"
---
# <a name="systemphotorelatedsoundfile-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Релатедсаундфиле

Политика метаданных фотографии для свойства [System. photo. релатедсаундфиле](../properties/props-system-photo-relatedsoundfile.md) .

### <a name="pkey"></a>PKEY

\_Релатедсаундфиле фото на PKEY \_

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ LPWSTR

### <a name="input-type"></a>Тип входных данных

Строка.

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                          | Формат диска |
|-------|-------------------------------|-------------|
| 1     | /APP1/IFD/EXIF/{ushort = 40964} | ascii       |
| 2     | /КСМП/ексиф: Релатедсаундфиле    | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                          | Формат диска |
|-------|-------------------------------|-------------|
| 1     | /APP1/IFD/EXIF/{ushort = 40964} | ascii       |
| 2     | /КСМП/ексиф: Релатедсаундфиле    | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                          |
|-------|-------------------------------|
| 1     | /APP1/IFD/EXIF/{ushort = 40964} |
| 2     | /КСМП/ексиф: Релатедсаундфиле    |



 

### <a name="tiff-policy"></a>Политика TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                           | Формат диска |
|-------|--------------------------------|-------------|
| 1     | /ИФД/ексиф/{ушорт = 40964}       | ascii       |
| 2     | /ИФД/КСМП/ексиф: Релатедсаундфиле | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                           | Формат диска |
|-------|--------------------------------|-------------|
| 1     | /ИФД/ексиф/{ушорт = 40964}       | ascii       |
| 2     | /ИФД/КСМП/ексиф: Релатедсаундфиле | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                           |
|-------|--------------------------------|
| 1     | /ИФД/ексиф/{ушорт = 40964}       |
| 2     | /ИФД/КСМП/ексиф: Релатедсаундфиле |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Релатедсаундфиле](../properties/props-system-photo-relatedsoundfile.md)
</dt> </dl>

 

 
