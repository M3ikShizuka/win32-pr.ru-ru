---
description: в Windows 7 и более поздних версиях можно добавлять команды в папку с помощью Desktop.ini. Дополнительные сведения о Desktop.ini файлах см. в статье Настройка папок с помощью Desktop.ini.
ms.assetid: F03AB35D-FBFE-46C2-A37F-F70C18219B9A
title: Реализация пользовательских команд для папок с помощью Desktop.ini
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f49b3f12d51848d08e6480d4180a3768b807703e5655e3fcfcddffcdaf16b734
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120111784"
---
# <a name="how-to-implement-custom-verbs-for-folders-through-desktopini"></a>Реализация пользовательских команд для папок с помощью Desktop.ini

в Windows 7 и более поздних версиях можно добавлять команды в папку с помощью Desktop.ini. Дополнительные сведения о Desktop.ini файлах см. [в статье Настройка папок с помощью Desktop.ini](how-to-customize-folders-with-desktop-ini.md).

> [!Note]  
> Desktop.ini файлы всегда должны быть помечены как   +  **скрытые** системой, чтобы они не отображались для пользователей.

 

Чтобы добавить пользовательские команды для папок с помощью файла Desktop.ini, выполните следующие действия.

## <a name="instructions"></a>Инструкции

### <a name="step-1"></a>Шаг 1.

Создайте папку, которая помечена как доступная **только для чтения** или как **система**.

### <a name="step-2"></a>Шаг 2.

Создайте файл Desktop.ini, содержащий \[ . Шеллклассинфо \] директорикласс = ProgID папки.

### <a name="step-3"></a>Шаг 3.

В реестре создайте **классы hKey \_ с \_ корневой** \\ **папкой ProgID** со значением канусефордиректори. Значение Канусефордиректори позволяет избежать неправильного использования ProgID, которые не участвуют в реализации пользовательских команд для папок с помощью Desktop.ini.

### <a name="step-4"></a>Шаг 4.

Добавьте команды в подключе ProgID **папки** , например:

```
HKEY_CLASSES_ROOT
   CustomFolderType
      Shell
         MyVerb
            command
               (Default) = %SystemRoot%\system32\notepad.exe %1\desktop.ini
```

## <a name="remarks"></a>Remarks

> [!Note]  
> Эти команды могут быть глаголами по умолчанию. в этом случае двойной щелчок папки активирует команду.

 

 

 



