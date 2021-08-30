---
description: Если действие Инсталлвалидате обнаруживает, что установка файла используется, отображает диалоговое окно Филесинусе и записывает в журнал следующие сведения.
ms.assetid: 59237d2c-6dda-4edc-bbaf-39c6b4c221b9
title: Ведение журнала запросов на перезагрузку
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ae5131d5662b4064538a9ae80936d6a02e74edbe44a725d5dd27754a9a2e845c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120043064"
---
# <a name="logging-of-reboot-requests"></a>Ведение журнала запросов на перезагрузку

Если [действие инсталлвалидате](installvalidate-action.md) обнаруживает, что установка файла используется, отображает [диалоговое окно филесинусе](filesinuse-dialog.md) и записывает в журнал следующие сведения.

``` syntax
Info 1603. The file E:\testdb\Test\CustAct1.dll is being held in use
by the following process: Name: test, Id: 137, Window Title: 'Test'.
```

Если установщик обнаруживает, что будет перезаписывать файл, который используется, он записывает в журнал следующие сведения.

``` syntax
Info 1603. The file E:\testdb\Test\CustAct2.dll is being held in use.

Info 1903.Scheduling reboot operation: Deleting file [filename]. Must 
reboot to complete operation.
```

\[Токен filename \] может фактически содержать путь к файлу с расширением радиальными базисными функциями. В этом случае файл. радиальными базисными функциями фактически является исходным файлом, регистрируемым сообщением 1603, которое было переименовано в радиальными базисными функциями-файл. Файл, который используется, сначала переименовывается с расширением радиальными базисными функциями, а затем удаляется.

Чтобы получить дополнительные сведения о том, почему установщик пытается перезаписать этот конкретный файл, можно использовать параметр подробного ведения журнала. Используйте \_ значение verbose инсталллогмоде в вызове [**мсиенаблелог**](/windows/desktop/api/Msi/nf-msi-msienableloga) или используйте параметр verbose Output в [параметрах командной строки](command-line-options.md). В этом случае записываются следующие сведения.

``` syntax
MSI (s) (D0:F0): File: E:\testdb\Test\CustAct2.dll;  Overwrite;  
REINSTALLMODE specifies all files to be overwritten
```

В журнал будет включено сообщение, например "существующий файл имеет более раннюю версию" или "существующий файл поврежден (Недопустимая контрольная сумма)".

 

 



