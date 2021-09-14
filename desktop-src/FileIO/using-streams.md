---
description: Пример кода, демонстрирующий использование базовых потоков файловой системы NTFS.
ms.assetid: 9cd5f418-404c-40f5-aa51-ef4d2a5f238e
title: использование Потоки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 04edc73a3524d45eeead4cd6c0d508925e6caa5e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057764"
---
# <a name="using-streams"></a>использование Потоки

В примере в этом разделе показано, как использовать базовые потоки файловой системы NTFS.

В этом примере создается файл с именем "TestFile" и размером 16 байт. Однако файл также имеет дополнительный тип потока:: $DATA с именем Stream, который добавляет дополнительные 23 байта, не сообщаемые операционной системой. Поэтому при просмотре свойства Размер файла для файла отображается только размер потока Default:: $DATA для файла.


```C++
#include <windows.h>
#include <stdio.h>

void main( )
 {
  HANDLE hFile, hStream;
  DWORD dwRet;

  hFile = CreateFile( TEXT("TestFile"), // Filename
                      GENERIC_WRITE,    // Desired access
                      FILE_SHARE_WRITE, // Share flags
                      NULL,             // Security Attributes
                      OPEN_ALWAYS,      // Creation Disposition
                      0,                // Flags and Attributes
                      NULL );           // OVERLAPPED pointer
  if( hFile == INVALID_HANDLE_VALUE )
   {
    printf( "Cannot open TestFile\n" );
    return;
   }
  else
   {
    WriteFile( hFile,              // Handle
               "This is TestFile", // Data to be written
               16,                 // Size of data, in bytes
               &dwRet,             // Number of bytes written
               NULL );             // OVERLAPPED pointer
    CloseHandle( hFile );
    hFile = INVALID_HANDLE_VALUE;
   }

  hStream = CreateFile( TEXT("TestFile:Stream"), // Filename
                        GENERIC_WRITE,           // Desired access
                        FILE_SHARE_WRITE,        // Share flags
                        NULL,                    // Security Attributes
                        OPEN_ALWAYS,             // Creation Disposition
                        0,                       // Flags and Attributes
                        NULL );                  // OVERLAPPED pointer
  if( hStream == INVALID_HANDLE_VALUE )
    printf( "Cannot open TestFile:Stream\n" );
  else
   {
    WriteFile( hStream,                   // Handle
               "This is TestFile:Stream", // Data to be written
               23,                        // Size of data
               &dwRet,                    // Number of bytes written
               NULL);                     // OVERLAPPED pointer
    CloseHandle( hStream );
    hStream = INVALID_HANDLE_VALUE;
   }
}
```



Если ввести в командной строке **тип TestFile** , он отобразит следующие выходные данные:

``` syntax
This is TestFile
```

Однако если ввести слова **типа TestFile: Stream**, выдается следующая ошибка:

Неверный синтаксис имени файла, имени каталога или метки тома ".

Чтобы просмотреть содержимое файла TestFile: Stream, используйте одну из следующих команд:

**Дополнительные < TestFile: Stream**

**Дополнительные < TestFile: Stream: $DATA**

Отображаемый текст выглядит следующим образом:

``` syntax
This is TestFile:Stream
```

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Потоки файлов](file-streams.md)
</dt> </dl>

 

 



