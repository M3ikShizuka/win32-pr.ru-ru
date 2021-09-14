---
description: Функция Михандлиррор является примером функции инструмента, используемой для вывода сообщения об ошибке и выхода из вызывающей программы.
ms.assetid: 7b28509f-a77f-4b60-90d4-18edaa6d1a2d
title: михандлиррор
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 047c9642a1b19c2af4a6e5ef2134ca305c472c09
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173187"
---
# <a name="myhandleerror"></a>михандлиррор

Функция **михандлиррор** является примером функции инструмента, используемой для вывода сообщения об ошибке и выхода из вызывающей программы. Примеры нескольких функций CryptoAPI в [справочнике по шифрованию](cryptography-reference.md) и более расширенные примеры [использования криптографии](using-cryptography.md) реализуют эту функцию. Для реальных приложений может потребоваться более сложная возможность обработки ошибок.


```C++
#include <stdio.h>
#include <tchar.h>
#include <windows.h>

void MyHandleError(LPTSTR psz)
{
    _ftprintf(stderr, TEXT("An error occurred in the program. \n"));
    _ftprintf(stderr, TEXT("%s\n"), psz);
    _ftprintf(stderr, TEXT("Error number %x.\n"), GetLastError());
    _ftprintf(stderr, TEXT("Program terminating. \n"));
    exit(1);
} // End of MyHandleError

```



 

 



