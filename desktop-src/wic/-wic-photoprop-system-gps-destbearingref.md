---
description: Политика метаданных фотографии для свойства System. GPS. Дестбеарингреф.
ms.assetid: d1c8b3cc-ed52-43ca-a0ba-045a2c5fe274
title: Политика метаданных фотографии System. GPS. Дестбеарингреф
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2f00d3083459fe365fc54e81dc485ddd26887a46
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256486"
---
# <a name="systemgpsdestbearingref-photo-metadata-policy"></a>Политика метаданных фотографии System. GPS. Дестбеарингреф

Политика метаданных фотографии для свойства [System. GPS. дестбеарингреф](../properties/props-system-gps-destbearingref.md) .

### <a name="pkey"></a>PKEY

PKEY \_ GPS \_ дестбеарингреф

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

### <a name="jpeg-policies"></a>Политики JPEG

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                        | Формат диска |
|-------|-----------------------------|-------------|
| 1     | /APP1/IFD/GPS/{ushort = 23}   | ascii       |
| 2     | /КСМП/ексиф: Гпсдестбеарингреф | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                        | Формат диска |
|-------|-----------------------------|-------------|
| 1     | /APP1/IFD/GPS/{ushort = 23}   | ascii       |
| 2     | /КСМП/ексиф: Гпсдестбеарингреф | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| Порядок | Путь                        |
|-------|-----------------------------|
| 1     | /APP1/IFD/GPS/{ushort = 23}   |
| 2     | /КСМП/ексиф: гпсдестбеарингреф |



 

### <a name="tiff-policies"></a>Политики TIFF

### <a name="read-paths"></a>Пути чтения



| Порядок | Путь                            | Формат диска |
|-------|---------------------------------|-------------|
| 1     | /ИФД/ГПС/{ушорт = 23}            | ascii       |
| 2     | /ИФД/КСМП/ексиф: Гпсдестбеарингреф | Юникод     |



 

### <a name="write-paths"></a>Пути записи



| Порядок | Путь                            | Формат диска |
|-------|---------------------------------|-------------|
| 1     | /ИФД/ГПС/{ушорт = 23}            | ascii       |
| 2     | /ИФД/КСМП/ексиф: Гпсдестбеарингреф | Юникод     |



 

### <a name="remove-paths"></a>Удалить пути



| порядок | path                            |
|-------|---------------------------------|
| 1     | /ИФД/ГПС/{ушорт = 23}            |
| 2     | /ИФД/КСМП/ексиф: гпсдестбеарингреф |



 

## <a name="remarks"></a>Комментарии

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[System. GPS. Дестбеарингреф](../properties/props-system-gps-destbearingref.md)
</dt> </dl>

 

 
