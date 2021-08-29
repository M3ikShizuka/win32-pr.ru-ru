---
description: Политика метаданных фотографии для свойства System. photo. Камерасериалнумбер.
ms.assetid: 85f78f45-5e76-4d52-88a2-ac3c9e2b6a1e
title: Политика метаданных фото для System. photo. Камерасериалнумбер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9a730df8041534a377262d9bb55a19c9b109b35ab03e47d1b7e8cb88014987b5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118710141"
---
# <a name="systemphotocameraserialnumber-photo-metadata-policy"></a>Политика метаданных фото для System. photo. Камерасериалнумбер

Политика метаданных фотографии для свойства [System. photo. камерасериалнумбер](../properties/props-system-photo-cameraserialnumber.md) .

### <a name="pkey"></a>PKEY

\_Камерасериалнумбер фото на PKEY \_

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

Если файл имеет формат JPEG, обработчик будет читать, записывать и удалять данные из следующего пути:



| Номер | Путь                                   | Формат диска | Обязательно |
|-------|----------------------------------------|-------------|----------|
| 1     | /КСМП/микрософтфото: Камерасериалнумбер | Юникод     | Да      |



 

### <a name="precedence-of-paths-tiff"></a>Приоритет путей (TIFF)

Если файл имеет формат TIFF, обработчик будет читать, записывать и удалять данные из следующего пути.



| Номер | Путь                                       | Формат диска | Обязательно |
|-------|--------------------------------------------|-------------|----------|
| 1     | /ИФД/КСМП/микрософтфото: Камерасериалнумбер | Юникод     | Да      |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. photo. Камерасериалнумбер](../properties/props-system-photo-cameraserialnumber.md)
</dt> </dl>

 

 
