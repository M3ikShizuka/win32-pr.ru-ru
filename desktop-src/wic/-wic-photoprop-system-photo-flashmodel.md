---
description: Политика метаданных фотографии для свойства System. photo. Флашмодел.
ms.assetid: ef322823-1b87-40ea-a5e3-e7551f14e44d
title: Политика метаданных фото для System. photo. Флашмодел
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 01ade3769cb0d852239af84b769b85d5b3849589
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458499"
---
# <a name="systemphotoflashmodel-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Флашмодел

Политика метаданных фотографии для свойства [System. photo. флашмодел](../properties/props-system-photo-flashmodel.md) .

### <a name="pkey"></a>PKEY

\_Флашмодел фото на PKEY \_

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

### <a name="precedence-of-paths-jpeg"></a>Приоритет путей (JPEG)

Если файл имеет формат JPEG, обработчик будет использовать следующий путь при чтении или записи данных.



| Порядок | Путь                           | Формат диска | Формат данных | Обязательно |
|-------|--------------------------------|-------------|-------------|----------|
| 1     | /КСМП/микрософтфото: Флашмодел | Юникод     |             | Да      |



 

### <a name="precedence-of-paths-tiff"></a>Приоритет путей (TIFF)

Если файл имеет формат TIFF, то при чтении или записи данных обработчик будет использовать следующий порядок приоритета.



| Порядок | Путь                               | Формат диска | Формат данных | Обязательно |
|-------|------------------------------------|-------------|-------------|----------|
| 1     | /ИФД/КСМП/микрософтфото: Флашмодел | Юникод     |             | Да      |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Флашмодел](../properties/props-system-photo-flashmodel.md)
</dt> </dl>

 

 
