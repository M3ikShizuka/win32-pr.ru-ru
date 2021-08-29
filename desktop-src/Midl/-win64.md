---
title: /Win64, параметр
description: Параметр/Win64 направляет компилятор MIDL для создания файлов заглушек или файла библиотеки типов для 64-разрядной среды. Примечание. Этот параметр устарел.
ms.assetid: 6f4780d3-6415-42af-a8ee-3884a8cebe26
keywords:
- MIDL/Win64 Switch
topic_type:
- apiref
api_name:
- /win64
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 963510db9f170a890797ebd3fffee4af9c270616b5d92b2a2333a47850311c30
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119913634"
---
# <a name="win64-switch"></a>/Win64, параметр

Параметр **/Win64** направляет компилятор MIDL для создания файлов заглушек или файла библиотеки типов для 64-разрядной среды.

> [!Note]  
> Этот параметр устарел. Используйте вместо него параметр [**/ia64**](-ia64.md) или [**/AMD64**](-amd64.md) . Параметр **/Win64** эквивалентен параметру **/ia64** .

 

``` syntax
midl /win64
```

## <a name="switch-options"></a>Параметры коммутатора

Этот параметр не имеет параметров.

## <a name="remarks"></a>Remarks

Параметр **/Win64** эквивалентен заданию параметра [**/env**](-env.md) для Win64.

> [!Note]  
> невозможно использовать MIDL.exe для создания 64-разрядного tlb на Windows 2000.

 

## <a name="see-also"></a>См. также

<dl> <dt>

[**/env**](-env.md)
</dt> <dt>

[**/ia64**](-ia64.md)
</dt> <dt>

[**/amd64**](-amd64.md)
</dt> </dl>

 

 




