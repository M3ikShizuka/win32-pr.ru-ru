---
description: файл WiFeatur.vbs VBScript предоставляется в Windows SDK компонентов для установщик Windows разработчиков.
ms.assetid: 797cb383-22c0-42b4-82c1-d5bcc3a8bafb
title: Функции списка
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 67e166401b514f1beec9c14c74aba7ca0601f446
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065422"
---
# <a name="list-features"></a>Функции списка

файл WiFeatur.vbs VBScript предоставляется в [Windows SDK компонентов для установщик Windows разработчиков](platform-sdk-components-for-windows-installer-developers.md). в этом примере показано, как использовать скрипт для перечисления функций в базе данных установщик Windows. в этом примере демонстрируется добавление временных столбцов в базу данных, доступную только для чтения установщик Windows.

В этом примере демонстрируются следующее:

-   [**Метод опендатабасе (объект установщика)**](installer-opendatabase.md), [**метод СоздатьЗапись**](installer-createrecord.md)и [**метод ластерроррекорд**](installer-lasterrorrecord.md) [**объекта установщика**](installer-object.md)
-   [**Метод Execute**](view-execute.md) и [**метод Fetch**](view-fetch.md) [**объекта View**](view-object.md)
-   [**Метод OpenView**](database-openview.md), [**свойство Таблеперсистент**](database-tablepersistent.md)и [**свойство примарикэйс**](database-primarykeys.md) [**объекта Database**](database-object.md)
-   Свойство [**FieldCount**](record-fieldcount.md), [**свойство IntegerData**](record-integerdata.md)и [**свойство StringData**](record-stringdata.md) [**объекта Record**](record-object.md)

для использования этого примера требуется CScript.exe или WScript.exe версии сервера сценариев Windows. Чтобы использовать CScript.exe для запуска этого образца, введите команду в командной строке, используя следующий синтаксис. Если первый аргумент имеет значение/?, отображается справка. или, если указано слишком мало аргументов. Чтобы перенаправить выходные данные в файл, завершите командную строку с помощью VBS > \[ *путь к файлу* \] . Пример возвращает значение 0 для успешного выполнения, 1, если вызывается Справка, и 2 в случае сбоя сценария.

**cscript WiFeatur.vbs \[ путь к \] \[ имени компонента базы данных\]**

укажите путь к базе данных установщик Windows. Укажите имя компонента. Он должен быть указан в столбце Feature [таблицы Features](feature-table.md). Если имя функции опущено, все функции перечислены как дерево компонентов. Если в \* качестве имени функции используется звездочка (), WiFeatur.vbs перечисляет все компоненты. Обратите внимание, что большие базы данных лучше отображать с помощью CScript, а не WScript.

дополнительные сведения см. в статье [установщик Windows примеры сценариев](windows-installer-scripting-examples.md) для дополнительных примеров сценариев. примеры служебных программ, для которых не требуется сервер сценариев Windows, см. в разделе [средства разработки установщик Windows](windows-installer-development-tools.md).

 

 



