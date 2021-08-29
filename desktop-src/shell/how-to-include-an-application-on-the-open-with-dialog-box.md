---
description: показано, как убедиться, что приложение отображается в меню открыть с помощью и в диалоговом окне для классических приложений и доступно в качестве приложения магазина Windows по умолчанию для указанных типов файлов.
ms.assetid: DFCC07A6-BED5-41A8-86DC-130082AE665A
title: Включение приложения в диалоговое окно «Открыть с помощью»
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2ad3d75d0eaf5ed60f2b9b6f4c468225e620c8d0bfbc8e14ed794a28f8f7098f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119714984"
---
# <a name="how-to-include-an-application-in-the-open-with-dialog-box"></a>Включение приложения в диалоговое окно «Открыть с помощью»

показано, как убедиться, что приложение отображается в меню **открыть с помощью** и в диалоговом окне для классических приложений и доступно в качестве приложения магазина Windows по умолчанию для указанных типов файлов.

## <a name="instructions"></a>Инструкции

### <a name="for-each-file-type-add-your-application-to-the-openwithprogids-registry-subkey"></a>Для каждого типа файлов добавьте приложение в подраздел реестра Опенвиспрогидс.

Добавьте идентификатор ProgID в качестве имени значения с типом значения REG \_ None или REG \_ SZ и пустой строкой в качестве значения данных.

в следующих примерах реестра показаны записи, связывающие InfoPath и Microsoft Visual Studio с типом XML-файла.

```
HKEY_CLASSES_ROOT
   .xml
      OpenWithProgids
         InfoPath.Document.3 REG_SZ
         VisualStudio.xml.10.0 REG_SZ
```

## <a name="remarks"></a>Remarks

Подключ **опенвиспрогидс** является предпочтительным для **опенвислист** для обнаружения приложения. Дополнительные сведения об этих подразделах см. в разделе [Настройка дополнительных подразделов и атрибутов расширения типов файлов](fa-file-types.md).

**опенвислист** предназначен только для устаревших приложений (должен быть только .exe) в операционных системах, предшествующих Windows XP.

```
HKEY_CLASSES_ROOT
   .xml
      OpenWithList
         AlternateProgram1.exe
         AlternateProgram2.exe
```

 

 



