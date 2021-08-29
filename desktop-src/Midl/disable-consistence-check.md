---
title: Атрибут disable_consistency_check
description: Направляет RPC, чтобы не применять проверку согласованности корреляции.
ms.assetid: 33ba331d-56e5-4965-a844-7780ea81623d
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: cc88112ac80462daa6c1babdd29799ccf05e33bb4edb52de1ffbbbb00e71352b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "117807229"
---
# <a name="disable_consistency_check-attribute"></a>отключить \_ \_ атрибут проверки согласованности

Направляет RPC, чтобы не применять проверку согласованности корреляции.

``` syntax
interface interface-name
{
  return-type function-name(
        [[attribute-list,] disable_consistency_check] param-type param-name
}
```

Для коррелированных параметров RPC будет обеспечивать передачу буфера, отличного от NULL, если значение переменной счетчика корреляций не равно null.

## <a name="example"></a>Пример

``` syntax
HRESULT PassString( [in] DWORD Length, [in, unique, string, 
    size_is( Length )]LPWSTR MyString );
```

Если параметр *MyString* имеет **значение NULL**, то RPC отклонит вызов, если для параметра length задано значение 0. Обратите внимание, что RPC допускает *длину* 0, в то время как *MyString* не имеет значение null, а RPC будет обрабатывать *MyString* как выделение буфера нулевой длины.

## <a name="remarks"></a>Remarks

Чтобы отключить эту проверку, IDL может содержать атрибут " \[ Отключить \_ проверку согласованности" \_ \] для параметра, typedef или типа указателя. Это позволит RPC не обеспечивать согласованность между указателем буфера и переменной корреляции для буфера, на который указывает параметр или указатель.

Чтобы отключить проверку согласованности для всей компиляции MIDL (и отключить принудительную проверку во всех случаях), можно использовать параметр командной строки MIDL [/бакквард \_ совместимого майбенулл \_ размера](-backward-compat.md) . Для этого необходимо, чтобы целевой объект компиляции MIDL был не меньше "Target NT60".

 

 




