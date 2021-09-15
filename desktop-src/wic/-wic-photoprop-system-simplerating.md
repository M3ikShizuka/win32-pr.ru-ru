---
description: Политика метаданных фотографии для свойства System. Симплератинг.
ms.assetid: d932a251-f238-4582-a1c4-cf4855f26fb3
title: Политика метаданных фотографии System. Симплератинг
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 63b91e41a0684c8e395992683e0a1d4fe43306a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344223"
---
# <a name="systemsimplerating-photo-metadata-policy"></a>Политика метаданных фотографии System. Симплератинг

Политика метаданных фотографии для свойства [System. симплератинг](../properties/props-system-simplerating.md) .

### <a name="pkey"></a>PKEY

PKEY \_ симплератинг

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ UI4

### <a name="input-propvariant-type"></a>Тип входного ПРОПВАРИАНТ

Может быть VT \_ UI1, VT \_ UI2 или VT \_ UI4. Целочисленное значение может находиться в диапазоне от 0 до 5.

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                     | Формат диска |
|-------|--------------------------|-------------|
| 1     | /APP1/IFD/{ushort = 18246} | ushort      |
| 2     | /КСМП/КСМП: Оценка          | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                     | Формат диска |
|-------|--------------------------|-------------|
| 1     | /APP1/IFD/{ushort = 18246} | ushort      |
| 2     | /КСМП/КСМП: Оценка          | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                     |
|-------|--------------------------|
| 1     | /APP1/IFD/{ushort = 18246} |
| 2     | /КСМП/КСМП: Оценка          |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                | Формат диска |
|-------|---------------------|-------------|
| 1     | /ИФД/{ушорт = 18246} | ushort      |
| 2     | /ИФД/КСМП/КСМП: Оценка | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                | Формат диска |
|-------|---------------------|-------------|
| 1     | /ИФД/{ушорт = 18246} | ushort      |
| 2     | /ИФД/КСМП/КСМП: Оценка | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                |
|-------|---------------------|
| 1     | /ИФД/{ушорт = 18246} |
| 2     | /ИФД/КСМП/КСМП: Оценка |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. Симплератинг](../properties/props-system-simplerating.md)
</dt> </dl>

 

 
