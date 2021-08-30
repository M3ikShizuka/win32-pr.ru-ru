---
title: Свойство Вебвиевфолдерконтентс. Фокуседитем (Шлдисп. h)
description: Вебвиевфолдерконтентс. Фокуседитем Property — возвращает объект FolderItem, представляющий элемент, имеющий фокус ввода.
ms.assetid: 84cf92ac-dadb-4741-8383-a8ae1d35d4e0
keywords:
- свойства фокуседитем устаревшей среды Windows
- свойства фокуседитем устаревшей среды Windows, объект вебвиевфолдерконтентс
- функции среды Windows вебвиевфолдерконтентс объектов прежних версий, свойство фокуседитем
topic_type:
- apiref
api_name:
- WebViewFolderContents.FocusedItem
api_location:
- Shell32.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0a4d9a22ac1529fc7f8f3880f53666e9835fae1088d3c7548abfa38a5f400061
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120114534"
---
# <a name="webviewfoldercontentsfocuseditem-property"></a>Вебвиевфолдерконтентс. Фокуседитем, свойство

Возвращает объект [**FolderItem**](../shell/folderitem.md) , представляющий элемент, имеющий фокус ввода.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
objFocusedItem = WebViewFolderContents.FocusedItem
```



## <a name="property-value"></a>Значение свойства

Переменная типа [IDispatch](/previous-versions/windows/desktop/api/oaidl/nn-oaidl-idispatch) , получающая объект элемента с сортировкой.

## <a name="examples"></a>Примеры

в следующем примере показано правильное использование этого свойства в JScript, внедренном в HTML.


```HTML
<html>
<head>

...

<script language="JavaScript">
    function fnWebViewFolderContentsFocusedItemJ()
    {
        var objFolderItem;

        objFolderItem = FileList.FocusedItem;
        if (objFolderItem != null)
        {
            alert(objFolderItem.Name);
        }
    }
</script>

</head>
<body>

...

<object id=FileList classid="clsid:1820FED0-473E-11D0-A96C-00C04FD705A2" tabIndex=1>
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



 

