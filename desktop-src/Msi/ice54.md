---
description: ICE54 проверяет наличие компонентов, использующих сопутствующий файл в качестве пути к ключу.
ms.assetid: 94fcabfe-4500-42f2-acea-13b9a6681ca6
title: ICE54
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 99df2ba90ccb44e33b67aaf8ecdcadc723e8d2fe
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127068047"
---
# <a name="ice54"></a>ICE54

ICE54 проверяет наличие компонентов, использующих сопутствующий файл в качестве пути к ключу.

Файл пути к ключу компонента не должен наследовать версию от другого файла. Это может привести к сбою установки некоторых файлов. Дополнительные сведения о сопутствующих файлах см. в [таблице File](file-table.md) .

## <a name="result"></a>Результат

ICE54 отправляет предупреждение, если какой-либо компонент имеет файл пути к ключу, который получает версию из другого файла.

## <a name="example"></a>Пример

ICE54 возвращает следующее предупреждение для показанного примера.

``` syntax
Component 'Component1' uses file 'File1' as its KeyPath, but the file's version is provided by the file 'File2'.
```

[Таблица Component](component-table.md) (частичная)



| Компонент  | attribute | Путь |
|------------|-----------|---------|
| Component1 | 0         | Файл1   |



 

[Таблица файлов](file-table.md) (частичная)



| Файл  | Версия | Язык |
|-------|---------|----------|
| Файл1 | Файл2   |          |
| Файл2 | 1.0.0.0 | 1033     |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по ICE](ice-reference.md)
</dt> </dl>

 

 



