---
title: Событие Error объекта Аксвиндовсмедиаплайер
description: событие error возникает, когда проигрыватель Windows Media элемент управления имеет условие ошибки.
ms.assetid: d28c18a9-c650-4169-989b-8727b7a5a831
keywords:
- событие Error объекта аксвиндовсмедиаплайер проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Error Event of the AxWindowsMediaPlayer Object
api_location:
- AxInterop.WMPLib.dll
api_type:
- Assembly
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6cfd3571538aa2cdd263a9f5d57e479e73818806
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242005"
---
# <a name="error-event-of-the-axwindowsmediaplayer-object"></a>Событие Error объекта Аксвиндовсмедиаплайер

событие error возникает, когда проигрыватель Windows Media элемент управления имеет условие ошибки.

``` syntax
[C#]
private void player_ErrorEvent(
  object sender,
  System.EventArgs e
)

[Visual Basic]
Private Sub player_ErrorEvent(  
  sender As Object,  
  e As System.EventArgs
) Handles player.ErrorEvent
```

## <a name="event-data"></a>Данные о событиях

Это событие не содержит данных.

## <a name="examples"></a>Примеры

В следующем примере создается обработчик событий для события Error для вывода текста описания первой ошибки в очереди ошибок. Объект Аксвмплиб. Аксвиндовсмедиаплайер представлен переменной с именем Player.


```CSharp
// Add a delegate for the Error event.
player.ErrorEvent += new EventHandler(player_ErrorEvent);

private void player_ErrorEvent(object sender, System.EventArgs e)
{
    // Get the description of the first error. 
    string errDesc = player.Error.get_Item(0).errorDescription;

    // Display the error description.
    System.Windows.Forms.MessageBox.Show(errDesc);
}
```


```VB

Public Sub player_ErrorEvent(ByVal sender As Object, ByVal e As System.EventArgs) Handles player.ErrorEvent

    &#39; Get the description of the first error. 
    Dim errDesc As String = player.Error.Item(0).errorDescription

    &#39; Display the error description.
    System.Windows.Forms.MessageBox.Show(errDesc)

End Sub
```





## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|----------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                          |
| Пространство имен<br/> | **аксвмплиб**<br/>                                                                                                    |
| Сборка<br/>  | <dl> <dt>AxInterop.WMPLib.dll (AxInterop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Аксвиндовсмедиаплайер (VB и C#)**](axwindowsmediaplayer-object--vb-and-c.md)
</dt> <dt>

[**Ивмперрор. Item (VB и C#)**](iwmperror-item--vb-and-c.md)
</dt> <dt>

[**Ивмперроритем. errorDescription (VB и C#)**](wmplibiwmperroritem-iwmperroritem-errordescription--vb-and-c.md)
</dt> </dl>

 

 





