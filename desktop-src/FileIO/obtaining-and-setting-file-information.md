---
description: Функции, используемые для получения и задания сведений о файле.
ms.assetid: 3b5fb709-c699-4651-8072-97210c8cf763
title: Получение и установка сведений о файле
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: aae2cdad8f5b00b0cf7663e7696a4e62e7fd523f543f0b7098316a4f562a1d96
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120130774"
---
# <a name="obtaining-and-setting-file-information"></a>Получение и установка сведений о файле

В следующих разделах описывается, как получить и задать сведения о файле.

## <a name="in-this-section"></a>В этом разделе



| Раздел                                                                                                             | Описание                                                                                                                                                                                                                                                                                   |
|-------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Получение сведений о типе файла](retrieving-file-type-information.md)<br/>                               | Функция [**жетфилетипе**](/windows/desktop/api/FileAPI/nf-fileapi-getfiletype) Извлекает тип файла: диск, символ (например, консоль), Pipe или Unknown.<br/>                                                                                                                                               |
| [Определение размера файла](determining-the-size-of-a-file.md)<br/>                                   | Функция [**GetFileSize**](/windows/desktop/api/FileAPI/nf-fileapi-getfilesize) получает размер файла.<br/>                                                                                                                                                                                                      |
| [Поиск одного или нескольких файлов](searching-for-one-or-more-files.md)<br/>                                 | Приложение может искать в текущем каталоге все имена файлов, соответствующие заданному шаблону, с помощью функций [**FindFirstFile**](/windows/desktop/api/FileAPI/nf-fileapi-findfirstfilea), [**финдфирстфиликс**](/windows/desktop/api/FileAPI/nf-fileapi-findfirstfileexa), [**FindNextFile**](/windows/desktop/api/FileAPI/nf-fileapi-findnextfilea)и [**финдклосе**](/windows/desktop/api/FileAPI/nf-fileapi-findclose) .<br/> |
| [Установка и получение метки времени файла](setting-and-getting-the-timestamp-of-a-file.md)<br/>         | Приложения могут извлекать и задавать дату и время создания файла, последнего изменения или последнего доступа с помощью функций [**функции getFileTime**](/windows/desktop/api/fileapi/nf-fileapi-getfiletime) и [**сетфилетиме**](/windows/desktop/api/fileapi/nf-fileapi-setfiletime) .<br/>                                                                         |
| [Определение кодовой страницы текущей кодировки](determining-the-current-character-set-code-page.md)<br/> | Функция [**AreFileApisANSI**](/windows/desktop/api/fileapi/nf-fileapi-arefileapisansi) определяет, использует ли функция файлового ввода-вывода кодовую страницу кодировки ANSI или OEM.<br/>                                                                                                                               |



 

 

