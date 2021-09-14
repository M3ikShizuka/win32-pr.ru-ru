---
description: Политика метаданных фотографии для свойства System. GPS. Широта.
ms.assetid: 0f8cea07-da96-4d2a-8444-6073b51e1236
title: Политика метаданных фотографии System. GPS. Широта
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5320869c1e8fd0d4b17bb17da455fc939bf44b9a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127375288"
---
# <a name="systemgpslatitude-photo-metadata-policy"></a>Политика метаданных фотографии System. GPS. Широта

Политика метаданных фотографии для свойства [System. GPS. Широта](../properties/props-system-gps-latitude.md) .

### <a name="pkey"></a>PKEY

PKEY \_ GPS, \_ Широта

### <a name="containers"></a>Контейнеры

JPEG, TIFF

### <a name="read-only"></a>Только для чтения

Да

### <a name="output-propvariant-type"></a>Тип выходного ПРОПВАРИАНТ

VT \_ вектор \| VT \_ R8

### <a name="conflict-resolution-policy"></a>Политика разрешения конфликтов

Это значение можно записать с помощью записи в System. GPS. Латитуденумератор и System. GPS. Латитудеденоминатор. Он не может быть записан напрямую. Выверяются значения из разных схем.

### <a name="jpeg-policy"></a>Политика JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                     | Формат диска |
|-------|--------------------------|-------------|
| 1     | /APP1/IFD/GPS/{ushort = 2} |             |
| 2     | /КСМП/ексиф: Гпслатитуде    |             |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                     | Формат диска |
|-------|--------------------------|-------------|
| 1     | /APP1/IFD/GPS/{ushort = 2} |             |
| 2     | /КСМП/ексиф: Гпслатитуде    |             |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                     |
|-------|--------------------------|
| 1     | /APP1/IFD/GPS/{ushort = 2} |
| 2     | /КСМП/ексиф: гпслатитуде    |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                      | Формат диска |
|-------|---------------------------|-------------|
| 1     | /ИФД/ГПС/{ушорт = 2}       |             |
| 2     | /ИФД/КСМП/ексиф: Гпслатитуде |             |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                      | Формат диска |
|-------|---------------------------|-------------|
| 1     | /ИФД/ГПС/{ушорт = 2}       |             |
| 2     | /ИФД/КСМП/ексиф: Гпслатитуде |             |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                      |
|-------|---------------------------|
| 1     | /ИФД/ГПС/{ушорт = 2}       |
| 2     | /ИФД/КСМП/ексиф: гпслатитуде |



 

## <a name="remarks"></a>Remarks

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. GPS. Широта](../properties/props-system-gps-latitude.md)
</dt> </dl>

 

 
