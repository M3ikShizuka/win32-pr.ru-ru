---
description: Политика метаданных фотографии для свойства System. Subject.
ms.assetid: 5ab7c74b-8a5e-4329-8a49-291470d406cc
title: Политика метаданных фотографии System. subject
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ceabbab95a52a1155db949dbc60b4525dd5f9d73
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344222"
---
# <a name="systemsubject-photo-metadata-policy"></a>Политика метаданных фотографии System. subject

Политика метаданных фотографии для свойства [System. subject](../properties/props-system-subject.md) .

### <a name="pkey"></a>PKEY

\_Тема PKEY

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ LPWSTR

### <a name="input-propvariant-type"></a>Тип входного ПРОПВАРИАНТ

VT \_ LPWSTR или VT \_ LPWSTR

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                     | Формат диска    |
|-------|--------------------------|----------------|
| 1     | /APP1/IFD/{ushort = 40095} | байт в Юникоде \_ |
| 2     | /APP1/IFD/{ushort = 270}   | ascii          |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                     | Формат диска    |
|-------|--------------------------|----------------|
| 1     | /APP1/IFD/{ushort = 40095} | байт в Юникоде \_ |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                     |
|-------|--------------------------|
| 1     | /APP1/IFD/{ushort = 40095} |
| 2     | /APP1/IFD/{ushort = 270}   |



 

### <a name="tiff-policy"></a>Политика TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                | Формат диска    |
|-------|---------------------|----------------|
| 1     | /ИФД/{ушорт = 40095} | байт в Юникоде \_ |
| 2     | /ИФД/{ушорт = 270}   | ascii          |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                | Формат диска    |
|-------|---------------------|----------------|
| 1     | /ИФД/{ушорт = 40095} | байт в Юникоде \_ |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                |
|-------|---------------------|
| 1     | /ИФД/{ушорт = 40095} |
| 2     | /ИФД/{ушорт = 270}   |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. subject](../properties/props-system-subject.md)
</dt> </dl>

 

 
