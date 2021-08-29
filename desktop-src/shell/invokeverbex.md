---
description: Выполняет команду для элемента оболочки.
ms.assetid: aac3f338-6074-4b1f-9b2f-e6206db52419
title: Шеллфолдеритем. Инвокевербекс, метод (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ShellFolderItem.InvokeVerbEx
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: 494c6b2926b204225b4afbf41b6271209f8be0abab4432f242ef4a5bd9c26cff
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119884424"
---
# <a name="shellfolderiteminvokeverbex-method"></a>Шеллфолдеритем. Инвокевербекс, метод

Выполняет команду для элемента оболочки.

## <a name="syntax"></a>Синтаксис


```JScript
iRetVal = ShellFolderItem.InvokeVerbEx(
  [ vVerb ],
  [ vArgs ]
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*вверб* \[ в необязательное\]
</dt> <dd>

Тип: **Variant**

**Значение типа Variant** , содержащее строку команды, соответствующую выполняемой команде. Оно должно быть одним из значений, возвращаемых свойством [**Name**](folderitemverb-name.md) элемента. Если команда не указана, выполняется команда по умолчанию.

</dd> <dt>

*варгс* \[ в необязательное\]
</dt> <dd>

Тип: **Variant**

**Вариант** , состоящий из строки с одним или несколькими аргументами команды, заданной параметром *вверб*. Формат этой строки зависит от конкретной команды.

</dd> </dl>

## <a name="remarks"></a>Remarks

Глагол — это строка, используемая для указания конкретного действия, которое поддерживает элемент. Как правило, вызов команды запускает связанное приложение. например, вызов команды **open** для файла .txt обычно открывает файл в текстовом редакторе, обычно Microsoft Блокнот. Объект [**фолдеритемвербс**](folderitemverbs.md) представляет коллекцию команд, связанных с элементом. Дальнейшее обсуждение глаголов см. в разделе [Запуск приложений](launch.md).

Этот метод аналогичен [**инвокеверб**](folderitem-invokeverb.md), но он позволяет задавать аргументы для команды, а также саму команду.

## <a name="examples"></a>Примеры

в следующих примерах показано правильное использование этого метода в JScript, VBScript и Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnFolderItem2InvokeVerbExJ()
    {
        var objShell = new ActiveXObject("shell.application");
        var objFolder2;
        var ssfWINDOWS = 36;
        
        objFolder2 = objShell.NameSpace(ssfWINDOWS);
        if (objFolder2 != null)
        {
            var objFolderItem;
            
            objFolderItem = objFolder2.ParseName("NOTEPAD.EXE");
            if (objFolderItem != null)
            {
                objFolderItem.InvokeVerbEx("open", "c:\\autoexec.bat");
            }
        }
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnFolderItemInvokeVerbExVB()
        dim objShell
        
        set objShell = CreateObject("shell.application")
        if (not objShell is nothing) then
            dim objFolder2
            dim ssfWINDOWS
                
            ssfWINDOWS = 36
            set objFolder2 = objShell.NameSpace(ssfWINDOWS)
            if (not objFolder2 is nothing) then
                dim objFolderItem
                        
                set objFolderItem = objFolder2.Self
                if (not objFolderItem is nothing) then
                    objFolderItem.InvokeVerbEx()
                end if
                set objFolderItem = nothing
            end if
            set objFolder2 = nothing
        end if
        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnFolderItem2InvokeVerbExVB()
    Dim objShell   As Shell
    Dim objFolder2 As Folder2
    Dim ssfWINDOWS As Long
    
    ssfWINDOWS = 36
    Set objShell = New Shell
    Set objFolder2 = objShell.NameSpace(ssfWINDOWS)
        If (Not objFolder2 Is Nothing) Then
            Dim objFolderItem2 As Object
            
            Set objFolderItem2 = objFolder2.ParseName("NOTEPAD.EXE")
                If (Not objFolderItem2 Is Nothing) Then
                    objFolderItem2.InvokeVerbEx ("open")
                Else
                    'FolderItem object returned nothing.
                End If
            Set objFolderItem2 = Nothing
        Else
            'Folder object returned nothing.
        End If
    Set objFolder2 = Nothing
    Set objShell = Nothing
End Sub
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 5,0 или более поздняя)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**шеллфолдеритем**](shellfolderitem-object.md)
</dt> <dt>

[**инвокеверб**](folderitem-invokeverb.md)
</dt> </dl>

 

 




