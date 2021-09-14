---
description: Политика метаданных фотографии для свойства System. photo. Транскодедфорсинк.
ms.assetid: 1869d845-6264-425a-ab3e-e0a9f942961a
title: Политика метаданных фото для System. photo. Транскодедфорсинк
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a5884ad469fcf7b5dffc8c4ad14f0ee5ff90cd07
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127251788"
---
# <a name="systemphototranscodedforsync-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Транскодедфорсинк

Политика метаданных фотографии для свойства [System. photo. транскодедфорсинк](../properties/props-system-photo-transcodedforsync.md) .

### <a name="pkey"></a>PKEY

\_Транскодедфорсинк фото на PKEY \_

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

Логическое значение VT \_

### <a name="input-type"></a>Тип входных данных

Логическое.

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                                  | Формат диска  |
|-------|---------------------------------------|--------------|
| 1     | /APP1/IFD/{ushort = 18248}              | bool, \_ UShort |
| 2     | /КСМП/микрософтфото: Транскодедфорсинк |              |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                                  | Формат диска  |
|-------|---------------------------------------|--------------|
| 1     | /APP1/IFD/{ushort = 18248}              | bool, \_ UShort |
| 2     | /КСМП/микрософтфото: Транскодедфорсинк |              |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                                  |
|-------|---------------------------------------|
| 1     | /APP1/IFD/{ushort = 18248}              |
| 2     | /КСМП/микрософтфото: транскодедфорсинк |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                                      | Формат диска  |
|-------|-------------------------------------------|--------------|
| 1     | /ИФД/{ушорт = 18248}                       | bool, \_ UShort |
| 2     | /ИФД/КСМП/микрософтфото: Транскодедфорсинк |              |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                                      | Формат диска  |
|-------|-------------------------------------------|--------------|
| 1     | /ИФД/{ушорт = 18248}                       | bool, \_ UShort |
| 2     | /ИФД/КСМП/микрософтфото: Транскодедфорсинк |              |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                                      |
|-------|-------------------------------------------|
| 1     | /ИФД/{ушорт = 18248}                       |
| 2     | /ИФД/КСМП/микрософтфото: транскодедфорсинк |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Транскодедфорсинк](../properties/props-system-photo-transcodedforsync.md)
</dt> </dl>

 

 
