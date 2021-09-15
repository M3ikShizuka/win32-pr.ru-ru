---
description: Политика метаданных фотографии для свойства System. photo. Фокалленгсинфилм.
ms.assetid: 3ad63a7a-5ced-4e7f-a4a0-e1463f3d3fa3
title: Политика метаданных фото для System. photo. Фокалленгсинфилм
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5df46f3e52c447cb7902fe3cce2da201dae16d9c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460175"
---
# <a name="systemphotofocallengthinfilm-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Фокалленгсинфилм

Политика метаданных фотографии для свойства [System. photo. фокалленгсинфилм](../properties/props-system-photo-focallengthinfilm.md) .

### <a name="pkey"></a>PKEY

PKEY \_ фокалленгсинфилм

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ UI4

### <a name="input-type"></a>Тип входных данных

UShort

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                            | Формат диска |
|-------|---------------------------------|-------------|
| 1     | /APP1/IFD/EXIF/{ushort = 41989}   | ushort      |
| 2     | /КСМП/ексиф: FocalLengthIn35mmFilm | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                            | Формат диска |
|-------|---------------------------------|-------------|
| 1     | /APP1/IFD/EXIF/{ushort = 41989}   | ushort      |
| 2     | /КСМП/ексиф: FocalLengthIn35mmFilm | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                            |
|-------|---------------------------------|
| 1     | /APP1/IFD/EXIF/{ushort = 41989}   |
| 2     | /КСМП/ексиф: focallengthin35mmfilm |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                                | Формат диска |
|-------|-------------------------------------|-------------|
| 1     | /ИФД/ексиф/{ушорт = 41989}            | ushort      |
| 2     | /ИФД/КСМП/ексиф: FocalLengthIn35mmFilm | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                                | Формат диска |
|-------|-------------------------------------|-------------|
| 1     | /ИФД/ексиф/{ушорт = 41989}            | ushort      |
| 2     | /ИФД/КСМП/ексиф: FocalLengthIn35mmFilm | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                                |
|-------|-------------------------------------|
| 1     | /ИФД/ексиф/{ушорт = 41989}            |
| 2     | /ИФД/КСМП/ексиф: focallengthin35mmfilm |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Фокалленгсинфилм](../properties/props-system-photo-focallengthinfilm.md)
</dt> </dl>

 

 
