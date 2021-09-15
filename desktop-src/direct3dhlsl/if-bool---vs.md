---
title: Если bool — VS
description: Запускает if... else... endif — блок vs.
ms.assetid: d77e2f81-400c-4997-9c34-426b6e6f47be
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 261ff572cbaf519cc0099f3ab68d1a0becca706f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568927"
---
# <a name="if-bool---vs"></a>Если bool — VS

Запускает if... [else](else---vs.md)... [endif — блок VS](endif---vs.md) .

## <a name="syntax"></a>Синтаксис



| Если bool |
|---------|



 

где bool — номер регистра bool. См. раздел [Постоянный логический регистр](dx9-graphics-reference-asm-vs-registers-constant-boolean.md).

## <a name="remarks"></a>Remarks



| Версии шейдеров вершин | 1\_1 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|------------------------|------|------|------|-------|------|-------|
| Если bool                |      | x    | x    | x     | x    | x     |



 

Если исходный логический регистр в операторе If имеет значение true, выполняется код, заключенный в операторе if и соответствующий else. В противном случае код, заключенный в [else](else---vs.md)... выполняется инструкция [endif-VS](endif---vs.md) . Эта инструкция использует один слот инструкций.

Если блоки могут быть вложенными.

Блок if не может помешать блоку цикла.

## <a name="example"></a>Пример

Эта инструкция предоставляет условное статическое управление потоком.


```
defb b2, TRUE

...

if b2
// Instructions to run if b2 is nonzero

else
// Instructions to run otherwise

endif
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера вершин](dx9-graphics-reference-asm-vs-instructions.md)
</dt> <dt>

[else — VS](else---vs.md)
</dt> <dt>

[endif — VS](endif---vs.md)
</dt> </dl>

 

 




