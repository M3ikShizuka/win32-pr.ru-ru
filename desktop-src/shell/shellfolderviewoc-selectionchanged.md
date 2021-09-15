---
description: Указывает, что состояние выбора одного или нескольких элементов в представлении изменилось.
title: Событие Шеллфолдервиевок. SelectionChanged (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SelectionChanged
api_type:
- DllExport
api_location:
- Shell32.dll
ms.assetid: 85c37f4e-229f-4383-8218-10f8c2b0b8a0
ms.openlocfilehash: 53d6fc3eb6f13d136af603a3129ba75a46c3c6a6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460305"
---
# <a name="shellfolderviewocselectionchanged-event"></a>Шеллфолдервиевок. SelectionChanged, событие

Указывает, что состояние выбора одного или нескольких элементов в представлении изменилось.

## <a name="syntax"></a>Синтаксис


```JScript
function EventHandler()
{
    // Code to handle the event.
}

// Set the event property to the handler.
ShellFolderViewOC.SelectionChanged = EventHandler;
```



## <a name="parameters"></a>Параметры

Этот обработчик событий не имеет параметров.

## <a name="remarks"></a>Remarks

Укажите код обработки событий для этого события, как показано здесь.


```
 
Private Sub object_SelectionChanged()
    'Event handling code
End Sub
                
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 5,0 или более поздняя)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**шеллфолдервиевок**](shellfolderviewoc-object.md)
</dt> </dl>

 

 




