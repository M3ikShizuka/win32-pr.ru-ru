---
description: Возвращает или задает описание ссылки.
ms.assetid: d3a95281-fb1f-4fd4-9d26-2a6e10a36a86
title: Свойство Шелллинкобжект. Description (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ShellLinkObject.Description
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: aff08831bf194da5c7ce958e5a0746abdd533dc0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460302"
---
# <a name="shelllinkobjectdescription-property"></a>Шелллинкобжект. Description, свойство

Возвращает или задает описание ссылки.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```JScript
strDescription = ShellLinkObject.Description
ShellLinkObject.Description(sDescription) = strDescription
```



## <a name="property-value"></a>Значение свойства

Описание ссылки.

## <a name="examples"></a>Примеры

в следующем примере показано правильное использование этого свойства в JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellShellLinkObjectDescriptionJ()
    {
        var objShell = new ActiveXObject("shell.application");
        var objFolder;
        var ssfPROGRAMS = 2;
        
        objFolder = objShell.NameSpace(ssfPROGRAMS);
        if (objFolder != null)
        {
            var objFolderItem;
            
            objFolderItem = objFolder.ParseName("Internet Explorer.lnk");
            if (objFolderItem != null)
            {
                var objShellLink;
                
                objShellLink = objFolderItem.GetLink;
                if (objShellLink != null)
                {
                    var szDescription;
                    
                    // Get the description for the ShellLinkObject.
                    szDescription = objShellLink.Description;
                    alert(szDescription);
                    
                    // Set the description for the ShellLinkObject.
                    objShellLink.Description = "Test"
                }
            }
        }
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnShellLinkObjectDescriptionVB()
        dim objShell
        dim objFolder
        dim ssfPROGRAMS
        
        ssfPROGRAMS = 2
        set objShell = CreateObject("shell.application")
        set objFolder = objShell.NameSpace(ssfPROGRAMS)
            if (not objFolder is nothing) then
                dim objFolderItem
                
                set objFolderItem = objFolder.ParseName("Internet Explorer.lnk")
                    if (not objFolderItem is nothing) then
                        dim objShellLink
                        
                        set objShellLink = objFolderItem.GetLink
                            if (not objShellLink is nothing) then
                                dim szDescription
                                
                                'Get the description for the ShellLinkObject.
                                szDescription = objShellLink.Description
                                alert(szDescription)
                                
                                'Set the description for the ShellLinkObject.
                                objShellLink.Description = "Test"
                            end if
                        set objShellLink = nothing
                    end if
                set objFolderItem = nothing
            end if
        set objFolder = nothing
        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
rivate Sub fnShellLinkObjectDescriptionVB()
    Dim objShell  As Shell
    Dim objFolder As Folder
    
    Set objShell = New Shell
    Set objFolder = objShell.NameSpace(ssfPROGRAMS)
        If (Not objFolder Is Nothing) Then
            Dim objFolderItem As FolderItem
            
            Set objFolderItem = objFolder.ParseName("Internet Explorer.lnk")
                If (Not objFolderItem Is Nothing) Then
                    Dim objShellLink As ShellLinkObject
                    
                    Set objShellLink = objFolderItem.GetLink
                        If (Not objShellLink Is Nothing) Then
                            Dim szDescription As String
                            
                            'Get the description for the ShellLinkObject.
                            szDescription = objShellLink.Description
                            Debug.Print szDescription
                            
                            'Set the description for the ShellLinkObject.
                            objShellLink.Description = "Test"
                        End If
                    Set objShellLink = Nothing
                End If
            Set objFolderItem = Nothing
        End If
    Set objFolder = Nothing
    Set objShell = Nothing
End Sub
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional с SP3 \[ только для настольных приложений\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 5,0 или более поздняя)</dt> </dl> |



 

 




