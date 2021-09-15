---
title: Ивмпконтролс Куррентпоситионстринг, свойство
description: Свойство Куррентпоситионстринг получает текущую позицию в элементе мультимедиа в виде строки в формате чч мм СС (часы, минуты и секунды).
ms.assetid: cd28dafa-b6a4-4bed-aa5d-7e7be6af1426
keywords:
- проигрыватель Windows Media свойства куррентпоситионстринг
- проигрыватель Windows Media свойства куррентпоситионстринг, интерфейс ивмпконтролс
- проигрыватель Windows Media интерфейса ивмпконтролс, свойство куррентпоситионстринг
topic_type:
- apiref
api_name:
- IWMPControls.currentPositionString
- IWMPControls.get_currentPositionString
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 85e941fceb61e4f00393b05f96489ec7ac8e950f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127270416"
---
# <a name="iwmpcontrolscurrentpositionstring-property"></a>Свойство Ивмпконтролс:: Куррентпоситионстринг

Свойство **куррентпоситионстринг** получает текущую позицию в элементе мультимедиа в виде строки, отформатированной как чч: мм: СС (часы, минуты и секунды).

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.String currentPositionString {get;}
```


```VB

Public ReadOnly Property currentPositionString As System.String
```





## <a name="property-value"></a>Значение свойства

Форматированная **Строка System. String** , которая является текущей позицией.

## <a name="remarks"></a>Комментарии

Если размер элемента мультимедиа меньше часа, текущая позиция форматируется как MM: SS (минуты и секунды).

## <a name="examples"></a>Примеры

В следующем примере запускается таймер, который запускает событие с интервалом в 1 секунду. В обработчике событий таймера метка обновляется с помощью **куррентпоситионстринг**. Объект **аксвмплиб. аксвиндовсмедиаплайер** представлен переменной с именем Player.


```CSharp
// Set the timer to fire an event every second and start the timer.
timer.Interval = 1000;
timer.Start();

// Note:  Use the AxWindowsMediaPlayer.PlayStateChange event with a switch statement to
// determine when to start and stop the timer. 
   
// Update the text of the label with the currentPositionString.
private void TimerEventProcessor(object sender, System.EventArgs e)
{
    currentPositionLabel.Text = player.Ctlcontrols.currentPositionString;
}
```


```VB

' Set the timer to fire an event every second and start the timer.
timer.Interval = 1000
timer.Start()

&#39; Note:  Use the AxWindowsMediaPlayer.PlayStateChange event with a switch statement to
&#39; determine when to start and stop the timer. 

&#39; Update the text of the label with the currentPositionString.
Public Sub TimerEventProcessor(ByVal sender As Object, ByVal e As System.EventArgs) Handles timer.Tick

    currentPositionLabel.Text = player.Ctlcontrols.currentPositionString

End Sub
```





## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпконтролс (VB и C#)**](iwmpcontrols--vb-and-c.md)
</dt> <dt>

[**Ивмпконтролс. currentPosition (VB и C#)**](wmplibiwmpcontrols-iwmpcontrols-currentposition--vb-and-c.md)
</dt> </dl>

 

 





