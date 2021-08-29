---
description: сведения о методе Shell. рефрешмену, который обновляет содержимое меню. используется только с системами, предшествующими Windows XP.
ms.assetid: 1269c66d-61df-432d-9220-5ac975e3ad58
title: Метод Shell. Рефрешмену (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Shell.RefreshMenu
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: 57f3b40e699d575d8dda3df2e2bb9005742321e63d537bae1b2e7814f46a0f79
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120090144"
---
# <a name="shellrefreshmenu-method"></a>Shell. Рефрешмену, метод

Обновляет содержимое меню " **Пуск** ". используется только с системами, предшествующими Windows XP.

## <a name="syntax"></a>Синтаксис


```JScript
iRetVal = Shell.RefreshMenu()
```


```VB

Shell.RefreshMenu() As Integer
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="remarks"></a>Remarks

функциональные возможности, предоставляемые **рефрешмену** , автоматически обрабатываются в Windows XP и более поздних версиях. Не вызывайте этот метод в этой операционной системе.

## <a name="examples"></a>Примеры

В следующем примере показано использование **рефрешмену** . правильное использование отображается для JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellRefreshMenuJ()
    {
        var objShell = new ActiveXObject("shell.application");
        
        objShell.RefreshMenu();
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnShellRefreshMenuVB()
        dim objShell
        
        set objShell = CreateObject("shell.application")
        objShell.RefreshMenu

        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnShellRefreshMenuVB()
    Dim objShell As Shell
    
    Set objShell = New Shell
    objShell.RefreshMenu

    Set objShell = Nothing
End Sub
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                           |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                           |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 4,71 или более поздняя)</dt> </dl> |



 

 




