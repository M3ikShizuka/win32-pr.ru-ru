---
description: в этом разделе описывается, как приложение загружает модуль ресурсов Win32 PE на Windows Vista и более поздней версии или в более ранней версии операционной системы. Для освобождения модуля ресурсов включены вызовы.
ms.assetid: c9f126a7-315a-4856-80b3-aec02402a80e
title: Загрузка модуля ресурсов Win32 PE
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f3c4c1906a4fc09dc39b805e8ad5a875d96fae27
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055335"
---
# <a name="loading-a-win32-pe-resource-module"></a>Загрузка модуля ресурсов Win32 PE

в этом разделе описывается, как приложение загружает модуль ресурсов Win32 PE на Windows Vista и более поздней версии или в более ранней версии операционной системы. Для освобождения модуля ресурсов включены вызовы.

## <a name="load-the-resource-module-on-windows-vista-and-later"></a>загрузка модуля ресурсов в Windows Vista и более поздних версий

в Windows Vista и более поздних версиях приложение загружает модуль ресурсов с помощью вызова [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) или [**LoadLibraryEx**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibraryexa). Рекомендуемая операция — вызвать эту функцию с обоими указанными флагами. Ниже приведен пример кода приложения, который загружает модуль на основе системных параметров языка.


```C++
HMODULE hResModule = LoadLibraryEx(TEXT("Mymodule.dll"), 0,
                                   LOAD_LIBRARY_AS_DATAFILE | LOAD_LIBRARY_AS_IMAGE_RESOURCE);
// ... insert code here to call resource loading functions ...
FreeLibrary(hResModule);
```



## <a name="load-the-resource-module-on-pre-windows-vista-operating-systems"></a>загрузка модуля ресурсов в операционных системах, предшествующих Windows Vista

в операционных системах, предшествующих Windows Vista, приложение загружает модуль ресурсов на основе параметра языка, совместимого с целевой операционной системой, а также Windows Vista и более поздних версий. Для этого типа загрузки модуля приложение должно вызывать функции многоязыкового интерфейса пользователя [**лоадмуилибрари**](/windows/desktop/api/Muiload/nf-muiload-loadmuilibrarya) и [**фримуилибрари**](/windows/desktop/api/Muiload/nf-muiload-freemuilibrary).


```C++
#include "MuiLoad.h"
HMODULE hResModule = LoadMUILibrary(TEXT("Mymodule.dll"), MUI_LANGUAGE_NAME, 0);
// ... insert code here to call resource loading functions ...
FreeMUILibrary(hResModule);
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Поиск ресурсов Win32 PE](locating-win32-pe-resources.md)
</dt> <dt>

[MUI: пример Параметры Application-Specific (Windows Vista)](mui-application-specific-settings-sample-vista.md)
</dt> <dt>

[MUI: пример Параметры Application-Specific (до Windows Vista)](mui-application-specific-settings-sample-pre-vista.md)
</dt> </dl>

 

 
