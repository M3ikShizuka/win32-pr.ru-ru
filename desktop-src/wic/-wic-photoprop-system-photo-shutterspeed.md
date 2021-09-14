---
description: Политика метаданных фотографии для свойства System. photo. Шуттерспид.
ms.assetid: f320944c-978d-4a3c-9bf8-5c5652123e29
title: Политика метаданных фото для System. photo. Шуттерспид
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b8df8c9e7fda5643fed022f67c3b6b7846e7a72f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247528"
---
# <a name="systemphotoshutterspeed-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Шуттерспид

Политика метаданных фотографии для свойства [System. photo. шуттерспид](../properties/props-system-photo-shutterspeed.md) .

### <a name="pkey"></a>PKEY

\_Шуттерспид фото на PKEY \_

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Да

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ R8

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Это значение формируется из System. photo. Шуттерспиднумератор и System. photo. Шуттерспидденоминатор. Он не может быть записан напрямую. Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                          | Формат диска |
|-------|-------------------------------|-------------|
| 1     | /APP1/IFD/EXIF/{ushort = 37377} |             |
| 2     | /КСМП/ексиф: Шуттерспидвалуе   |             |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                          | Формат диска |
|-------|-------------------------------|-------------|
| 1     | /APP1/IFD/EXIF/{ushort = 37377} |             |
| 2     | /КСМП/ексиф: Шуттерспидвалуе   |             |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                          |
|-------|-------------------------------|
| 1     | /APP1/IFD/EXIF/{ushort = 37377} |
| 2     | /КСМП/ексиф: шуттерспидвалуе   |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                            | Формат диска |
|-------|---------------------------------|-------------|
| 1     | /ИФД/ексиф/{ушорт = 37377}        |             |
| 2     | /ИФД/КСМП/ексиф: Шуттерспидвалуе |             |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                            | Формат диска |
|-------|---------------------------------|-------------|
| 1     | /ИФД/ексиф/{ушорт = 37377}        |             |
| 2     | /ИФД/КСМП/ексиф: Шуттерспидвалуе |             |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                            |
|-------|---------------------------------|
| 1     | /ИФД/ексиф/{ушорт = 37377}        |
| 2     | /ИФД/КСМП/ексиф: шуттерспидвалуе |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Шуттерспид](../properties/props-system-photo-shutterspeed.md)
</dt> </dl>

 

 
