---
description: Ишеллдиспатч. Бровсефорфолдер — создает диалоговое окно, которое позволяет пользователю выбрать папку, а затем возвращает объект папки выбранной папки.
ms.assetid: 578C51C1-F59B-4604-A09B-62BA61225ABB
title: Ишеллдиспатч. Бровсефорфолдер, метод (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IShellDispatch.BrowseForFolder
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: ee6202c7029e2c27684e15d96dd6c38680cb0678
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257035"
---
# <a name="ishelldispatchbrowseforfolder-method"></a>Ишеллдиспатч. Бровсефорфолдер, метод

Создает диалоговое окно, которое позволяет пользователю выбрать папку, а затем возвращает объект [**папки**](folder.md) выбранной папки.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = IShellDispatch.BrowseForFolder(
  Hwnd,
  sTitle,
  iOptions,
  [ vRootFolder ]
)
```


```VB

IShellDispatch.BrowseForFolder( _
  ByVal Hwnd As Integer, _
  ByVal sTitle As BSTR, _
  ByVal iOptions As Integer, _
  [ ByVal vRootFolder As Variant ] _
) As FOLDER
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*HWND* \[ окне\]
</dt> <dd>

Тип: **Integer**

Маркер родительского окна диалогового поля. Это значение может быть равно 0.

</dd> <dt>

*ститле* \[ окне\]
</dt> <dd>

Тип: **[ **BSTR**](/previous-versions/windows/desktop/automat/bstr)**

**Строковое** значение, представляющее заголовок, отображаемый в диалоговом окне **Обзор** .

</dd> <dt>

*иоптионс* \[ окне\]
</dt> <dd>

Тип: **Integer**

**Целочисленное** значение, содержащее параметры для метода. Это может быть ноль или сочетание значений, перечисленных под элементом **улфлагс** структуры [**бровсеинфо**](/windows/desktop/api/shlobj_core/ns-shlobj_core-browseinfoa) .

</dd> <dt>

*врутфолдер* \[ в необязательное\]
</dt> <dd>

Тип: **Variant**

Корневая папка, используемая в диалоговом окне. Пользователь не может просматривать выше в дереве, чем эта папка. Если это значение не указано, в качестве корневой папки, используемой в диалоговом окне, используется рабочий стол. Это значение может быть строкой, указывающей путь к папке или одно из значений [**шеллспеЦиалфолдерконстантс**](/windows/desktop/api/Shldisp/ne-shldisp-shellspecialfolderconstants) . обратите внимание, что имена констант, найденные в **шеллспеЦиалфолдерконстантс** , доступны в Visual Basic, но не в VBScript или JScript. В таких случаях необходимо использовать числовые значения на своем месте.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

### <a name="jscript"></a>Язык JScript

Тип: **Папка \* \***

Ссылка на объект [**папки**](folder.md) выбранной папки.

### <a name="vb"></a>VB

Тип: **Папка \* \***

Ссылка на объект [**папки**](folder.md) выбранной папки.

## <a name="remarks"></a>Комментарии

Этот метод реализован и доступен через метод [**Shell. бровсефорфолдер**](shell-browseforfolder.md) .

## <a name="examples"></a>Примеры

в следующих примерах используется **бровсефорфолдер** для вывода окна обзора под названием «Example», корнем которого является папка Windows. сведения об использовании отображаются для JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellBrowseForFolderJ()
    {
        var objShell = new ActiveXObject("shell.application");
        var ssfWINDOWS = 36;
        var objFolder;
        
        objFolder = objshell.BrowseForFolder(0, "Example", 0, ssfWINDOWS);
        if (objFolder != null)
        {
            // Add code here.
        }
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnShellBrowseForFolderVB()
        dim objShell
        dim ssfWINDOWS
        dim objFolder
        
        ssfWINDOWS = 36
        set objShell = CreateObject("shell.application")
            set objFolder = objshell.BrowseForFolder(0, "Example", 0, ssfWINDOWS)
                if (not objFolder is nothing) then
                    'Add code here.
                end if
            set objFolder = nothing
        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnShellBrowseForFolderVB()
    Dim objShell   As Shell
    Dim ssfWINDOWS As Long
    Dim objFolder  As Folder
    
    ssfWINDOWS = 36
    Set objShell = New Shell
        Set objFolder = objshell.BrowseForFolder(0, "Example", 0, ssfWINDOWS)
            If (Not objFolder Is Nothing) Then
                'Add code here
            End If
        Set objFolder = Nothing
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



 

 
