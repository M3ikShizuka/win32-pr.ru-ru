---
description: 'Windows Функции API, управляющие символами, обычно реализуются в одном из трех форматов:'
ms.assetid: e7698f0b-dbcb-4cd0-9cb5-23a26edb966a
title: Юникод в Windows API
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5686a7f65edefb11458374b7f72262448becd6d1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254980"
---
# <a name="unicode-in-the-windows-api"></a>Юникод в Windows API

Windows Функции API, управляющие символами, обычно реализуются в одном из трех форматов:

-   универсальная версия, которая может быть скомпилирована либо для Windows кодовых страниц, либо для юникода
-   версия [кодовой страницы Windows](code-pages.md) с буквой "A", используемой для обозначения "ANSI"
-   Версия в [Юникоде](unicode.md) с буквой "W", используемой для обозначения "Wide"

Некоторые новые функции поддерживают только версии Юникода. Дополнительные сведения см. в разделе [соглашения для прототипов функций](conventions-for-function-prototypes.md).

В следующих разделах рассматриваются типы данных в Юникоде и их использование в функциях и сообщениях. использование ресурсов, имен файлов и аргументов командной строки; методы преобразования между различными типами строк.

-   [Автоматическое преобразование сообщений](automatic-message-translation.md)
-   [Кодировки, используемые в именах файлов](character-sets-used-in-file-names.md)
-   [Аргументы командной строки](command-line-arguments.md)
-   [Правила обозначения прототипов функций](conventions-for-function-prototypes.md)
-   [Стандартные функции C](standard-c-functions.md)
-   [Различия строковых функций](string-function-differences.md)
-   [Преобразование между строковыми типами](translation-between-string-types.md)
-   [Windows Data Types for Strings](windows-data-types-for-strings.md) (Типы данных Windows для работы со строками)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[О кодировке Юникод и кодировке](about-unicode-and-character-sets.md)
</dt> </dl>

 

 



