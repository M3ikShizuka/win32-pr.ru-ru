---
description: Политика метаданных фотографии для свойства System. Author.
ms.assetid: 2de9c452-93be-40a4-a72b-5da590534dfd
title: Политика метаданных фотографии System. Author
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 817fbea6a05b182bdb401f7ed623c0ebe94bbf63
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573147"
---
# <a name="systemauthor-photo-metadata-policy"></a>Политика метаданных фотографии System. Author

Политика метаданных фотографии для свойства [System. Author](../properties/props-system-author.md) .

### <a name="pkey"></a>PKEY

\_Автор PKEY

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ Векторная \| \_ LPWSTR

### <a name="input-propvariant-type"></a>Тип входного ПРОПВАРИАНТ

\_Предпочтителен VT Vector \| VT \_ , но \_ также принимается VT LPWSTR.

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                             | Формат диска    |
|-------|----------------------------------|----------------|
| 1     | /APP1/IFD/{ushort = 315}           | ascii          |
| 2     | /app13/irb/8bimiptc/iptc/by-line |                |
| 3     | /КСМП/ &lt; ксмпсек &gt; DC: Creator    | Юникод        |
| 4     | /app13/irb/8bimiptc/iptc/by-line |                |
| 5     | /APP1/IFD/{ushort = 40093}         | байт в Юникоде \_ |
| 6     | /КСМП/Тифф: исполнитель                 | Юникод        |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                             | Формат диска    |
|-------|----------------------------------|----------------|
| 1     | /КСМП/ &lt; ксмпсек &gt; DC: Creator    | Юникод        |
| 2     | /КСМП/Тифф: исполнитель                 | Юникод        |
| 3     | /app13/irb/8bimiptc/iptc/by-line |                |
| 4     | /APP1/IFD/{ushort = 315}           | ascii          |
| 5     | /APP1/IFD/{ushort = 40093}         | байт в Юникоде \_ |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                             |
|-------|----------------------------------|
| 1     | /КСМП/ДК: Creator                  |
| 2     | /КСМП/Тифф: исполнитель                 |
| 3     | /app13/irb/8bimiptc/iptc/by-line |
| 4     | /APP1/IFD/{ushort = 315}           |
| 5     | /APP1/IFD/{ushort = 40093}         |



 

### <a name="tiff-policy"></a>Политика TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                              | Формат диска    |
|-------|-----------------------------------|----------------|
| 1     | /ИФД/{ушорт = 315}                 | ascii          |
| 2     | /ифд/иптк/би-лине                 |                |
| 3     | /ИФД/КСМП/ &lt; ксмпсек &gt; DC: Creator | Юникод        |
| 4     | /ифд/иптк/би-лине                 |                |
| 5     | /ИФД/{ушорт = 40093}               | байт в Юникоде \_ |
| 6     | /ifd/irb/8bimiptc/iptc/by-line    |                |
| 7     | /ИФД/КСМП/Тифф: исполнитель              | Юникод        |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                              | Формат диска    |
|-------|-----------------------------------|----------------|
| 1     | /ИФД/КСМП/ &lt; ксмпсек &gt; DC: Creator | Юникод        |
| 2     | /ИФД/КСМП/Тифф: исполнитель              | Юникод        |
| 3     | /ифд/иптк/би-лине                 |                |
| 4     | /ИФД/{ушорт = 315}                 | \_вектор ASCII  |
| 5     | /ИФД/{ушорт = 40093}               | байт в Юникоде \_ |
| 6     | /ифд/иптк/би-лине                 |                |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                           |
|-------|--------------------------------|
| 1     | /ИФД/КСМП/ДК: Creator            |
| 2     | /ИФД/КСМП/Тифф: исполнитель           |
| 3     | /ифд/иптк/би-лине              |
| 4     | /ifd/irb/8bimiptc/iptc/by-line |
| 5     | /ИФД/{ушорт = 315}              |
| 6     | /ИФД/{ушорт = 40093}            |



 

### <a name="remarks"></a>Комментарии

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System.Author](../properties/props-system-author.md)
</dt> </dl>

 

 
