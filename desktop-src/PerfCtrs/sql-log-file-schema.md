---
description: приложения могут использовать PDH для извлечения счетчиков производительности из журналов SQL, а также для извлечения форматированных или необработанных счетчиков непосредственно из базы данных с помощью запросов SQL.
ms.assetid: 89515dd9-2d65-4b19-bb7a-ef9e7d146caa
title: SQL Схема файла журнала
ms.topic: article
ms.date: 08/17/2020
ms.openlocfilehash: 33b988194a8fda4a99f713e0026aeaddb65e9c26
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055123"
---
# <a name="sql-log-file-schema"></a>SQL Схема файла журнала

> [!IMPORTANT]
> поддержка PDH для баз данных ODBC SQL может быть изменена или недоступна в будущем.

приложения могут использовать интерфейсы api PDH для чтения и записи данных счетчиков производительности в совместимых базах данных ODBC SQL, а затем выполняют дальнейшую обработку с помощью запросов SQL. в этом разделе описывается схема SQL, используемая для хранения счетчиков производительности. Эти сведения можно использовать для создания пользовательских представлений и отчетов. Схема состоит из следующих трех таблиц:

- [**каунтердата**](counterdata.md)
- [**каунтердетаилс**](counterdetails.md)
- [**дисплайтоид**](displaytoid.md)

> [!NOTE]
> поддержка PDH для баз данных odbc SQL работает только с драйверами odbc SQL, поддерживающими расширения для выполнения [операций копирования (BCP)](/sql/relational-databases/native-client-odbc-extensions-bulk-copy-functions/sql-server-driver-extensions-bulk-copy-functions).
