---
description: Shell. Ежектпк метод — извлекает компьютер из стыковочного узла. это то же самое, что щелчок меню и выбор пункта извлечь компьютер, если компьютер поддерживает эту команду.
ms.assetid: eaba3dce-8fea-453f-90c2-4a9b5cb05ecc
title: Метод Shell. Ежектпк (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Shell.EjectPC
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: 5ec08aaa82d2f752fa06537434adede86b9d5a3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247978"
---
# <a name="shellejectpc-method"></a>Shell. Ежектпк, метод

Извлекает компьютер из стыковочного узла. Это то же самое, что и при нажатии кнопки " **Пуск** " и выборе пункта " **извлечь компьютер**", если компьютер поддерживает эту команду.

## <a name="syntax"></a>Синтаксис


```JScript
Shell.EjectPC()
```


```VB

Shell.EjectPC()
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

### <a name="jscript"></a>Язык JScript

Этот метод не возвращает значение.

### <a name="vb"></a>VB

Этот метод не возвращает значение.

## <a name="examples"></a>Примеры

В следующем примере показано использование **ежектпк** . правильное использование отображается для JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellEjectPCJ()
    {
        var objShell = new ActiveXObject("shell.application");
        
        objShell.EjectPC();
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnShellEjectPCVB()
        dim objShell
        
        set objShell = CreateObject("shell.application")
        objShell.EjectPC

        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnShellEjectPCVB()
    Dim objShell As Shell
    
    Set objShell = New Shell
    objShell.EjectPC

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



 

 




