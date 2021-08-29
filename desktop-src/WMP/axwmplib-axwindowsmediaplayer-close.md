---
title: Аксвиндовсмедиаплайер. Close, метод
description: метод close закрывает текущий файл мультимедиа, останавливает воспроизведение в проигрыватель Windows Media и освобождает проигрыватель Windows Media ресурсов.
ms.assetid: 3e555086-c31c-42d7-b671-0fd824f66641
keywords:
- метод close проигрыватель Windows Media
- метод close проигрыватель Windows Media, класс аксвиндовсмедиаплайер
- класс аксвиндовсмедиаплайер проигрыватель Windows Media, метод close
topic_type:
- apiref
api_name:
- AxWindowsMediaPlayer.close
api_location:
- AxInterop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1cece6f4034a687a68cbd596bfe26a23c2fe70112c9e432c6f06b9065c1436c9
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119737084"
---
# <a name="axwindowsmediaplayerclose-method"></a>Аксвиндовсмедиаплайер. Close, метод

метод close закрывает текущий файл мультимедиа, останавливает воспроизведение в проигрыватель Windows Media и освобождает проигрыватель Windows Media ресурсов.

## <a name="syntax"></a>Синтаксис


```CSharp
public void close();
```


```VB

Public Sub close()
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

этот метод закрывает текущий файл мультимедиа, но не проигрыватель Windows Media самого себя.

## <a name="examples"></a>Примеры

в следующем примере создается кнопка, которая при нажатии останавливает воспроизведение в проигрыватель Windows Media и освобождает используемые ресурсы. Объект Аксвмплиб. Аксвиндовсмедиаплайер представлен переменной с именем Player.


```CSharp
private void closeIt_Click(object sender, System.EventArgs e)
{
    // Close the Player. 
    player.close();
}
```


```VB

Public Sub closeIt_Click(ByVal sender As Object, ByVal e As System.EventArgs) Handles closeIt.Click

    &#39; Close the Player. 
    player.close()

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
</dt> </dl>

 

 





