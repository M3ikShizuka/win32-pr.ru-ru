---
description: Указывает, что объект Шеллфолдервиев завершил перечисление содержимого папки.
title: Событие Шеллфолдервиевок. Енумдоне (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- EnumDone
api_type:
- DllExport
api_location:
- Shell32.dll
ms.assetid: 7baa5f58-62c2-406e-a81e-4ca9c446a756
ms.openlocfilehash: 00b0e58ed18ab0da9c3fa362da4b8e3e066cdcc4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579518"
---
# <a name="shellfolderviewocenumdone-event"></a>Шеллфолдервиевок. Енумдоне, событие

Указывает, что объект [**шеллфолдервиев**](shellfolderview.md) завершил перечисление содержимого папки.

## <a name="syntax"></a>Синтаксис


```JScript
function EventHandler()
{
    // Code to handle the event.
}

// Set the event property to the handler.
ShellFolderViewOC.EnumDone = EventHandler;
```



## <a name="parameters"></a>Параметры

Этот обработчик событий не имеет параметров.

## <a name="remarks"></a>Remarks

Объект [**шеллфолдервиев**](shellfolderview.md) должен перечислить содержимое папки, прежде чем она сможет ее отобразить. При наличии больших или расположенных в удаленной системе папок Этот процесс может занять несколько минут. В течение этого времени отображается анимированный рисунок фонарик, указывающий пользователю, что обработка выполняется по-разному. После перечисления будет вызвано событие **енумдоне** , и изображение фонарик заменяется содержимым папки.

Укажите код обработки событий для этого события, как показано здесь.


```
 
Private Sub object_EnumDone()
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

 

 




