---
title: Строки (RPC)
description: Три типа строк и удаленный вызов процедур (RPC).
ms.assetid: 186cabeb-ea3f-4213-ba71-53afe91e6e14
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 207e20b1c343ded17b5d62db2321bee380463f20
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461454"
---
# <a name="strings-rpc"></a>Строки (RPC)

Существует три типа строк, обозначенных следующими завершающими подстроками в символе формата.



| Тип                  | Substring |
|-----------------------|-----------|
| Строка символов      | CSTRING   |
| Строка расширенных символов | WSTRING   |
| Структура, доступная для строк | сстринг   |



 

### <a name="nonconformant-strings"></a>Несоответствующие строки

Примером несогласованной строки является **\[ строка \]** в массиве фиксированного размера.

``` syntax
FC_CSTRING | FC _WSTRING 
FC_PAD 
string_size<2>
```

### <a name="conformant-strings"></a>Согласованные строки

``` syntax
FC_C_CSTRING | FC_C_WSTRING
FC_PAD 
```

–или–

``` syntax
FC_C_CSTRING | FC_C_WSTRING 
FC_STRING_SIZED 
conformance_description<> 
```

Первый формат описывает общие строки, например **\[ строковый \]** аргумент Char \* . Строка с указанием размера имеет Последнее описание.

\_Описание соответствия<> является дескриптором корреляции и имеет 4 или 6 байт в зависимости от того, используется ли [**/robust**](/windows/desktop/Midl/-robust) .

### <a name="structure-strings"></a>Строки структуры

Ниже приведена несоответствующая структура строк.

``` syntax
FC_SSTRING 
element_size<1> 
number_of_elements<2>
```

Согласованная структура, поддерживающая строки:

``` syntax
FC_C_SSTRING 
element_size<1>
```

ни

``` syntax
FC_C_SSTRING 
elements_size<1> 
FC_STRING_SIZED FC_PAD 
conformance_description<>
```

Последнее описание предназначено для структуры, которая может иметь размер строк.

 

 