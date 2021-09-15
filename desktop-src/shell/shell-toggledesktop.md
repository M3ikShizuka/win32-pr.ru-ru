---
description: Shell. Тоггледесктоп-метод — отображает или скрывает Рабочий стол.
title: Метод Shell.ToggleDesktop (Shldisp.h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Shell.ToggleDesktop
api_type:
- COM
api_location:
- Shell32.dll
ms.assetid: BD07F7F2-A588-4189-95F4-3A8E2905E8F5
ms.openlocfilehash: 472f6141b8aaed47ac05c8eaf670a0d039ce5561
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460340"
---
# <a name="shelltoggledesktop-method"></a>Shell. Тоггледесктоп, метод

Отображает или скрывает Рабочий стол.

## <a name="syntax"></a>Синтаксис


```JScript
Shell.ToggleDesktop()
```


```VB

Shell.ToggleDesktop()
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

### <a name="jscript"></a>Язык JScript

Этот метод не возвращает значение.

### <a name="vb"></a>VB

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод действует так же, как кнопка " **Свернуть Рабочий стол** " на панели задач. Он либо скрывает все открытые окна для отображения рабочего стола, либо скрывает Рабочий стол, отображая все открытые окна. Метод **тоггледесктоп** не отображает пользовательский интерфейс, он просто вызывает действие Toggle.

## <a name="examples"></a>Примеры

в следующих примерах показано правильное использование **тоггледесктоп** для JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnIShellDispatch4ToggleDesktopJ()
    {
        var objShell = new ActiveXObject("shell.application");
        
        objShell.ToggleDesktop();
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnIShellDispatch4ToggleDesktopVB()
        dim objShell
        
        set objShell = CreateObject("shell.application")
            objShell.ToggleDesktop
        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnIShellDispatch4ToggleDesktopVB()
    Dim objShell As Shell
            
    Set objShell = New Shell
        objShell.ToggleDesktop
    Set objShell = Nothing
End Sub
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                                                   |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 6,0 или более поздняя)</dt> </dl> |



 

 




