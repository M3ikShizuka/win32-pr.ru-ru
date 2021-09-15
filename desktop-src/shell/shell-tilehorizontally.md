---
description: Мозаичное отображение всех окон на рабочем столе по горизонтали. этот метод действует аналогично щелчку правой кнопкой мыши панели задач и выбора плитки Windows горизонтально.
ms.assetid: b0e06766-1bd4-4744-81f3-139b018aa72c
title: Метод Shell. Тилехоризонталли (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Shell.TileHorizontally
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: e295d0a7847afc0cb405f3ab9141e54ae424e9e8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460346"
---
# <a name="shelltilehorizontally-method"></a>Shell. Тилехоризонталли, метод

Мозаичное отображение всех окон на рабочем столе по горизонтали. этот метод действует аналогично щелчку правой кнопкой мыши панели задач и выбора **плитки Windows горизонтально**.

## <a name="syntax"></a>Синтаксис


```JScript
iRetVal = Shell.TileHorizontally()
```


```VB

Shell.TileHorizontally() As Integer
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="examples"></a>Примеры

В следующем примере показано использование **тилехоризонталли** . правильное использование отображается для JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellTileHorizontallyJ()
    {
        var objShell = new ActiveXObject("shell.application");
        
        objShell.TileHorizontally();
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnShellTileHorizontallyVB()
        dim objShell
        
        set objShell = CreateObject("shell.application")
        objShell.TileHorizontally

        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnShellTileHorizontallyVB()
    Dim objShell As Shell
    
    Set objShell = New Shell
    objShell.TileHorizontally

    Set objShell = Nothing
End Sub
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                           |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                           |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 4,71 или более поздняя)</dt> </dl> |



 

 




