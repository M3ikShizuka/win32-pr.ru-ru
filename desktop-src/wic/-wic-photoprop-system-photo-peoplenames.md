---
description: Политика метаданных фотографии для свойства System. photo. Пеопленамес.
ms.assetid: 567d5542-fc7b-4d19-bc3c-b9d6e26e3387
title: Политика метаданных фото для System. photo. Пеопленамес
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5540356001cdd33bb7c0d3340534f9c69e230a5d
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122886447"
---
# <a name="systemphotopeoplenames-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Пеопленамес

Политика метаданных фотографии для свойства [System. photo. пеопленамес](../properties/props-system-photo-peoplenames.md) .

### <a name="pkey"></a>PKEY

\_Пеопленамес фото на PKEY \_

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Нет

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ Векторная \| \_ LPWSTR

### <a name="input-type"></a>Тип входных данных

стрингмулти

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | путь                                                           | Формат диска |
|-------|----------------------------------------------------------------|-------------|
| 1     | /КСМП/ &lt; ксмпструкт &gt; MP: RegionInfo/ &lt; Ксмпбаг &gt; МПРИ: regions | ushort      |



 

### <a name="write-paths"></a>Пути записи

Это свойство нельзя записать с помощью политики метаданных.

### <a name="remove-paths"></a>Удалить пути



| Порядок | путь                                |
|-------|-------------------------------------|
| 1     | /КСМП/ &lt; ксмпструкт &gt; MP: RegionInfo |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | путь                                                               | Формат диска |
|-------|--------------------------------------------------------------------|-------------|
| 1     | /ИФД/КСМП/ &lt; ксмпструкт &gt; MP: RegionInfo/ &lt; Ксмпбаг &gt; МПРИ: regions | ushort      |



 

### <a name="write-paths"></a>Пути записи

Это свойство нельзя записать с помощью политики метаданных.

### <a name="remove-paths"></a>Удалить пути



| Порядок | путь                                    |
|-------|-----------------------------------------|
| 1     | /ИФД/КСМП/ &lt; ксмпструкт &gt; MP: RegionInfo |



 

## <a name="remarks"></a>Комментарии

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Программоде](../properties/props-system-photo-programmode.md)
</dt> </dl>

 

 
