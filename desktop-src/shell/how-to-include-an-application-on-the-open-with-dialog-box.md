---
description: показано, как убедиться, что приложение отображается в меню открыть с помощью и в диалоговом окне для классических приложений и доступно в качестве приложения магазина Windows по умолчанию для указанных типов файлов.
ms.assetid: DFCC07A6-BED5-41A8-86DC-130082AE665A
title: Включение приложения в диалоговое окно «Открыть с помощью»
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 218dcbfe6dc34770208c017f0e13cfda7686430c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127262544"
---
# <a name="how-to-include-an-application-in-the-open-with-dialog-box"></a>Включение приложения в диалоговое окно «Открыть с помощью»

показано, как убедиться, что приложение отображается в меню **открыть с помощью** и в диалоговом окне для классических приложений и доступно в качестве приложения магазина Windows по умолчанию для указанных типов файлов.

## <a name="instructions"></a>Instructions

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

 

 



