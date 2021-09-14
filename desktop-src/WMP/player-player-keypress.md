---
title: Событие Player. KeyPress
description: Событие KeyPress возникает при нажатии и отпускании клавиши. | Событие Player. KeyPress
ms.assetid: fc51dfd3-7968-464a-a4e2-669ffcb52a59
keywords:
- проигрыватель Windows Media события KeyPress
- событие KeyPress проигрыватель Windows Media, класс Player
- класс проигрывателя проигрыватель Windows Media, событие KeyPress
topic_type:
- apiref
api_name:
- Player.KeyPress
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c78b72dd703c13019c71b23af53790aa974927f1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064450"
---
# <a name="playerkeypress-event"></a>Событие Player. KeyPress

Событие **KeyPress** возникает при нажатии и отпускании клавиши.

## <a name="syntax"></a>Синтаксис


```JScript
Player.KeyPress(
  nKeyAscii
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*нкэйасЦии* 
</dt> <dd>

**Number** (**целое** число), задающее стандартный числовой код ANSI для символа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Это событие возникает, когда нажатие клавиши приводит к вводу любого печатного символа клавиатуры, клавиши CTRL в сочетании с символом из стандартного алфавита или одного из нескольких специальных символов, а также клавишей Ввод или BACKSPACE.

значение параметров события задается проигрыватель Windows Media, и к нему можно получить доступ или передать в метод в импортированном JScriptном файле, используя имя параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

**проигрыватель Windows Media 10 Mobile:** Это событие не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





