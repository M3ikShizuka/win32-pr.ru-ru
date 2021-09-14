---
description: Файлы описания библиотеки — это XML-файлы, определяющие библиотеки.
ms.assetid: 12F6E6AE-2776-408c-B9AC-E885BE93C27F
title: Схема описания библиотеки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2bfbaa8401468a6bab79cf4bccc5d7d4cd0ff7bb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256993"
---
# <a name="library-description-schema"></a>Схема описания библиотеки

Файлы описания библиотеки — это XML-файлы, определяющие библиотеки. библиотеки объединяют элементы из локальных и удаленных мест хранения в единое представление в Windows Explorer. Файлы описания библиотеки соответствуют схеме описания библиотеки и сохраняются в \* файлах. Library-MS.

Этот раздел состоит из следующих подразделов.

-   [Общие сведения о схеме описания библиотеки](#overview-of-the-library-description-schema)
-   [Управление версиями пространства имен](#namespace-versioning)
-   [Пример файла описания библиотеки](#example-of-a-library-description-file)
-   [Связанные темы](#related-topics)

## <a name="overview-of-the-library-description-schema"></a>Общие сведения о схеме описания библиотеки

Библиотеки содержат файлы, которые хранятся в одном или нескольких местах хранения. Библиотеки на самом деле не хранят эти файлы; Вместо этого они отслеживают папки, содержащие файлы, и предоставляют пользователям доступ к файлам и их упорядочение различными способами. Например, пользователь может иметь музыкальные файлы в нескольких папках на локальном жестком диске, а также на внешнем жестком диске. С помощью **библиотеки музыки** пользователь может одновременно получить доступ ко всем файлам и отсортировать их по имени исполнителя или названию альбома в виде одной группы.

Схема описания библиотеки состоит из трех основных частей, описанных в следующей таблице.



| Часть                        | Описание                                                                                                                                                |
|-----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Общие сведения о библиотеке | сведения о библиотеке, такие как имя, владелец, версия, значок, который Windows Explorer может использовать при отображении библиотеки для пользователя.                   |
| Свойства библиотеки          | Одно или несколько свойств, описывающих библиотеку. Эти пользовательские свойства относятся к библиотеке.                                                     |
| Расположения библиотек           | Один или несколько соединителей поиска, которые указывают места хранения для включения в библиотеку. Каждое из этих расположений также может иметь уникальный набор свойств. |



 

файлы библиотек в Windows 7 хранятся в известных папках, FOLDERID \_ библиотеках. по умолчанию папка FOLDERID \_ librarys находится в каталоге% USERPROFILE% \\ AppData \\ роуминга \\ Microsoft \\ Windows \\ librarys.

## <a name="namespace-versioning"></a>Управление версиями пространства имен

Версии формата файла описания библиотеки ( \* . Library-MS) отправляются путем изменения пространства имен. для Windows 7 формат файла имеет следующее пространство имен по умолчанию: https://schemas.microsoft.com/windows/2009/library .

Однако версии содержимого библиотеки отправляются с помощью элемента [ &lt; Version &gt; ](schema-library-version.md) в конкретном файле описания библиотеки.

## <a name="example-of-a-library-description-file"></a>Пример файла описания библиотеки

Ниже приведен пример файла описания библиотеки, который определяет библиотеку для файлов документов.


```
<?xml version="1.0" encoding="UTF-8"?>
<libraryDescription xmlns="http://schemas.microsoft.com/windows/2009/library">
    <name>@shell32.dll,-34575</name>
    <ownerSID>S-1-5-21-379071477-2495173225-776587366-1000</ownerSID>
    <version>1</version>
    <isLibraryPinned>true</isLibraryPinned>
    <iconReference>imageres.dll,-1002</iconReference>
    <templateInfo>
        <folderType>{7d49d726-3c21-4f05-99aa-fdc2c9474656}</folderType>
    </templateInfo>
    <searchConnectorDescriptionList>
        <searchConnectorDescription publisher="Microsoft" product="Windows">
            <description>@shell32.dll,-34577</description>
            <isDefaultSaveLocation>true</isDefaultSaveLocation>
            <simpleLocation>
                <url>knownfolder:{FDD39AD0-238F-46AF-ADB4-6C85480369C7}</url>
                <serialized>MBAAAEAFCAAA...MFNVAAAAAA</serialized>
            </simpleLocation>
        </searchConnectorDescription>
        <searchConnectorDescription publisher="Microsoft" product="Windows">
            <description>@shell32.dll,-34579</description>
            <isDefaultNonOwnerSaveLocation>true</isDefaultNonOwnerSaveLocation>
            <simpleLocation>
                <url>knownfolder:{ED4824AF-DCE4-45A8-81E2-FC7965083634}</url>
                <serialized>MBAAAEAFCAAA...HJIfK9AAAAAA</serialized>
            </simpleLocation>
        </searchConnectorDescription>
    </searchConnectorDescriptionList>
</libraryDescription>
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Элемент Фолдертипе (схема библиотеки)](schema-library-foldertype.md)
</dt> <dt>

[Элемент Иконреференце (схема библиотеки)](schema-library-iconreference.md)
</dt> <dt>

[Элемент Ислибрарипиннед (схема библиотеки)](schema-library-islibrarypinned.md)
</dt> <dt>

[Элемент Либраридескриптион (схема библиотеки)](schema-librarydescription.md)
</dt> <dt>

[Элемент Name (схема библиотеки)](schema-library-name.md)
</dt> <dt>

[Элемент ownerSID (схема библиотеки)](schema-library-ownersid.md)
</dt> <dt>

[Элемент Property (схема библиотеки)](schema-library-property.md)
</dt> <dt>

[Элемент Пропертисторе (схема библиотеки)](schema-library-propertystore.md)
</dt> <dt>

[Элемент Сеарчконнектордескриптион (схема библиотеки)](schema-library-searchconnectordescription.md)
</dt> <dt>

[Элемент Сеарчконнектордескриптионлист (схема библиотеки)](schema-library-searchconnectordescriptionlist.md)
</dt> <dt>

[Элемент Темплатеинфо (схема библиотеки)](schema-library-templateinfo.md)
</dt> <dt>

[Элемент Version (схема библиотеки)](schema-library-version.md)
</dt> <dt>

[Схема описания соединителя поиска](../search/search-sconn-desc-schema-entry.md)
</dt> </dl>

 

 
