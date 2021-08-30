---
title: Ивмпконтролс Фастфорвард, метод
description: Метод Фастфорвард запускает быстрое воспроизведение элемента мультимедиа в прямом направлении. | Ивмпконтролс Фастфорвард, метод
ms.assetid: 44609d63-1d1a-489c-ac17-60b6d3ddc588
keywords:
- проигрыватель Windows Media метода фастфорвард
- проигрыватель Windows Media метода фастфорвард, интерфейс ивмпконтролс
- проигрыватель Windows Media интерфейса ивмпконтролс, метод фастфорвард
topic_type:
- apiref
api_name:
- IWMPControls.fastForward
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f283ef56f3831f58b8d57f3d172ad3b80163ee62fdaa24b05bdca02c68cafcf5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120031334"
---
# <a name="iwmpcontrolsfastforward-method"></a>Метод Ивмпконтролс:: Фастфорвард

Метод **фастфорвард** запускает быстрое воспроизведение элемента мультимедиа в прямом направлении.

## <a name="syntax"></a>Синтаксис


```CSharp
public void fastForward();
```


```VB

Public Sub fastForward()
Implements IWMPControls.fastForward
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Метод **фастфорвард** воспроизводит клип в пять раз после обычной скорости. Вызов **фастфорвард** эквивалентен указанию 5,0 для скорости путем установки свойства **ивмпсеттингс. rate** . если частота впоследствии изменилась или если вызывается **ивмпконтролс. play** или **ивмпконтролс. остановка** , проигрыватель Windows Media прекращает быструю пересылку.

Метод **фастфорвард** не работает для широковещательных трансляций и определенных типов носителей. Чтобы определить, можно ли выполнить быструю пересылку клипа, передайте значение **System. String** "фастфорвард" в свойство **ивмпконтролс. Available** (метод **ивмпконтролс. Get- \_ Available** в C#).

## <a name="examples"></a>Примеры

В следующем примере **фастфорвард** используется для перемотки текущего элемента мультимедиа в ответ на событие щелчка кнопки. Объект **аксвмплиб. аксвиндовсмедиаплайер** представлен переменной с именем Player.


```CSharp
private void fastForwardButton_Click(object o, System.EventArgs args)
{
    // To get all of the available functionality of the player controls, cast the
    // value returned by player.Ctlcontrols to a WMPLib.IWMPControls3 interface. 
    WMPLib.IWMPControls3 controls = (WMPLib.IWMPControls3)player.Ctlcontrols;

    // Check first to be sure the operation is valid.
    if (controls.get_isAvailable("fastForward"))
    {
        controls.fastForward();
    }
}
```


```VB

Public Sub fastForwardButton_Click(ByVal sender As Object, ByVal e As System.EventArgs) Handles fastForwardButton.Click

    &#39; To get all of the available functionality of the player controls, Dim the
    &#39; value returned by player.Ctlcontrols as a WMPLib.IWMPControls3 interface. 
    Dim controls As WMPLib.IWMPControls3 = player.Ctlcontrols

    &#39; Check first to be sure the operation is valid.
    If (controls.isAvailable(&quot;fastForward&quot;)) Then

        controls.fastForward()

    End If

End Sub
```





## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Интерфейс Ивмпконтролс (VB и C#)**](iwmpcontrols--vb-and-c.md)
</dt> <dt>

[**Ивмпконтролс. доступ (VB и C#)**](iwmpcontrols-isavailable--vb-and-c.md)
</dt> <dt>

[**Ивмпконтролс. Play (VB и C#)**](wmplibiwmpcontrols-iwmpcontrols-play--vb-and-c.md)
</dt> <dt>

[**Ивмпконтролс. останавливаться (VB и C#)**](wmplibiwmpcontrols-iwmpcontrols-stop--vb-and-c.md)
</dt> <dt>

[**Ивмпсеттингс. rate (VB и C#)**](wmplibiwmpsettings-iwmpsettings-rate--vb-and-c.md)
</dt> </dl>

 

 





