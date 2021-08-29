---
description: Метод Ишеллдиспатч. NameSpace — создает и возвращает объект Folder для указанной папки.
ms.assetid: CEA73705-1C27-4138-86C4-1715016E2ED8
title: Метод Ишеллдиспатч. NameSpace (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IShellDispatch.NameSpace
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: d870d6e4de6ac43c66a275bd9f5be54880badae8b7a575f13587c11c5c9b757f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119942364"
---
# <a name="ishelldispatchnamespace-method"></a>Ишеллдиспатч. NameSpace, метод

Создает и возвращает объект [**Folder**](folder.md) для указанной папки.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = IShellDispatch.NameSpace(
  vDir
)
```


```VB

IShellDispatch.NameSpace( _
  ByVal vDir As Variant _
) As Folder
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*vDir* \[ окне\]
</dt> <dd>

Тип: **Variant**

Папка, для которой создается объект [**папки**](folder.md) . Это может быть строка, указывающая путь к папке или одно из значений [**шеллспеЦиалфолдерконстантс**](/windows/desktop/api/Shldisp/ne-shldisp-shellspecialfolderconstants) . обратите внимание, что имена констант, найденные в **шеллспеЦиалфолдерконстантс** , доступны в Visual Basic, но не в VBScript или JScript. В таких случаях необходимо использовать числовые значения на своем месте.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

### <a name="jscript"></a>Язык JScript

Тип: **[ **Папка**](folder.md)\*\***

Ссылка на объект [**Folder**](folder.md) для указанной папки. Если папка не была создана, это значение возвращает значение **null**.

### <a name="vb"></a>VB

Тип: **[ **Папка**](folder.md)\*\***

Ссылка на объект [**Folder**](folder.md) для указанной папки. Если папка не была создана, это значение возвращает значение **null**.

## <a name="remarks"></a>Remarks

Этот метод реализован и доступен через метод [**Shell. Namespace**](shell-namespace.md) .

## <a name="examples"></a>Примеры

в следующих примерах показано использование [**пространства имен**](shell-namespace.md) в JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellNameSpaceJ()
    {
        var objShell = new ActiveXObject("shell.application");
        var objFolder;
        var ssfWINDOWS = 36
        
        objFolder = objShell.NameSpace(ssfWINDOWS);
        if (objFolder != null)
        {
            alert(objFolder.Title);
        }
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnShellNameSpaceVB()
        dim objShell
        dim objFolder
        
        set objShell = CreateObject("shell.application")
        set objFolder = objShell.NameSpace("C:\")

        if (not objFolder is nothing) then
            alert(objFolder.Title)
        end if

        set objFolder = nothing
        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnShellNameSpaceVB()
    Dim objShell  As Shell
    Dim objFolder As Folder

    Set objShell = New Shell
    Set objFolder = objShell.NameSpace(ssfPERSONAL)

    If (Not objFolder Is Nothing) Then
        Debug.Print objFolder.Title
    End If

    Set objFolder = Nothing
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



 

 




