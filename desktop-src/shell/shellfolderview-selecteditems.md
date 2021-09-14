---
description: Шеллфолдервиев. SelectedItems, метод возвращает объект Фолдеритемс, представляющий все выбранные элементы в представлении.
title: Метод ShellFolderView.SelectedItems (Shldisp.h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ShellFolderView.SelectedItems
api_type:
- COM
api_location:
- Shell32.dll
ms.assetid: 1ee3bf2e-f9c9-47d9-a0f2-efedd69770c5
ms.openlocfilehash: 485eda530adc4955abb27899d67ac0900eb0a910
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460315"
---
# <a name="shellfolderviewselecteditems-method"></a>Шеллфолдервиев. SelectedItems, метод

Возвращает объект [**фолдеритемс**](folderitems.md) , представляющий все выбранные элементы в представлении.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = ShellFolderView.SelectedItems()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **фолдеритемс**](folderitems.md)\*\***

Ссылка на объект [**фолдеритемс**](folderitems.md) .

## <a name="remarks"></a>Remarks

**SelectedItems** может быть вызван только в локальной системе. Он не будет работать при запуске на веб-странице по протоколу HTTP или UNC.

## <a name="examples"></a>Примеры

в следующем примере показано правильное использование этого метода в JScript, внедренном в HTML.


```JScript
<html>
<head>
<title></title>

<script language="JavaScript">
    function fnShellFolderViewSelectedItemsJ()
    {
        var objFolderItems;
        
        objFolderItems = WebOC.Document.SelectedItems();
        if (objFolderItems != null)
        {
            alert("Got FolderItems object.");
        }
    }
    
    function fnLoad()
    {
        var webOC;
        
        webOC = document.all("WebOC");
        webOC.Navigate("C:\\");
    }
</script>

</head>
<body onload="fnLoad()">
<object id="WebOC" 
        classid="clsid:8856F961-340A-11D0-A96B-00C04FD705A2"
        width=400
        height=400>
</object>
<br><br>
<INPUT id=SelectedItems 
       type=button 
       value=SelectedItems 
       name=SelectedItems 
       onclick="fnShellFolderViewSelectedItemsJ()">
</body>
</html>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                           |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                           |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 4,71 или более поздняя)</dt> </dl> |



 

 




