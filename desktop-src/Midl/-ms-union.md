---
title: ms_union Switch
description: '\_Параметр объединения/МС управляет выравниванием ОНД неинкапсулированных объединений. Обратите внимание, что этот атрибут предоставляется для обеспечения обратной совместимости.'
ms.assetid: 683d1498-6419-4600-ad5b-c0b6ea44a8e1
keywords:
- /ms_union параметр MIDL
topic_type:
- apiref
api_name:
- /ms_union
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 968618af5c2bb5b32ec14b293225bc09c2997aa5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144149"
---
# <a name="ms_union-switch"></a>\_коммутатор объединения/МС

Параметр **\_ объединения/МС** управляет выравниванием ОНД неинкапсулированных объединений.

> [!Note]  
> Этот атрибут предоставляется для обеспечения обратной совместимости. Не рекомендуется использовать в новом интерфейсе.

 

``` syntax
midl /ms_union
```

## <a name="switch-options"></a>Параметры коммутатора

Этот параметр не имеет параметров.

## <a name="remarks"></a>Remarks

Компилятор MIDL отражает поведение компилятора IDL использование-DCE для неинкапсулированных объединений. Однако, поскольку более ранние версии компилятора MIDL не сделали этого, коммутатор **/МС \_ Union** обеспечивает совместимость с интерфейсами, созданными в предыдущих версиях компилятора MIDL.

Функцию MS \_ Union можно использовать в качестве параметра командной строки (**/МС \_ Union**), атрибута интерфейса IDL или в качестве атрибута IDL-Type.

## <a name="examples"></a>Примеры

**MIDL- \_ файл/МС Union File. idl**

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Общий синтаксис командной строки MIDL](general-midl-command-line-syntax.md)
</dt> <dt>

[Файл определения интерфейса (IDL)](interface-definition-idl-file.md)
</dt> </dl>

 

 




