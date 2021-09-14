---
description: Политика метаданных фотографии для свойства System. photo. ФотометриЦинтерпретатион.
ms.assetid: ff36b2c3-8763-4640-a049-b5880fd26929
title: Политика метаданных фото для System. photo. ФотометриЦинтерпретатион
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 35b371ce9257d526f941f3fdb33949e8788a7112
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247537"
---
# <a name="systemphotophotometricinterpretation-photo-metadata-policy"></a>Политика метаданных фото для System. photo. ФотометриЦинтерпретатион

Политика метаданных фотографии для свойства [System. photo. фотометриЦинтерпретатион](../properties/props-system-photo-photometricinterpretation.md) .

### <a name="pkey"></a>PKEY

\_ФотометриЦинтерпретатион фото на PKEY \_

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Да

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ UI2

### <a name="input-type"></a>Тип входных данных

UShort

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                                | Формат диска |
|-------|-------------------------------------|-------------|
| 1     | /APP1/IFD/{ushort = 262}              | ushort      |
| 2     | /КСМП/Тифф: ФотометриЦинтерпретатион | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                                | Формат диска |
|-------|-------------------------------------|-------------|
| 1     | /APP1/IFD/{ushort = 262}              | ushort      |
| 2     | /КСМП/Тифф: ФотометриЦинтерпретатион | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                                |
|-------|-------------------------------------|
| 1     | /APP1/IFD/{ushort = 262}              |
| 2     | /КСМП/Тифф: фотометриЦинтерпретатион |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                                    | Формат диска |
|-------|-----------------------------------------|-------------|
| 1     | /ИФД/{ушорт = 262}                       | ushort      |
| 2     | /ИФД/КСМП/Тифф: ФотометриЦинтерпретатион | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                                    | Формат диска |
|-------|-----------------------------------------|-------------|
| 1     | /ИФД/{ушорт = 262}                       | ushort      |
| 2     | /ИФД/КСМП/Тифф: ФотометриЦинтерпретатион | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                                    |
|-------|-----------------------------------------|
| 1     | /ИФД/{ушорт = 262}                       |
| 2     | /ИФД/КСМП/Тифф: фотометриЦинтерпретатион |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. ФотометриЦинтерпретатион](../properties/props-system-photo-photometricinterpretation.md)
</dt> </dl>

 

 
