---
title: Событие Warning объекта Аксвиндовсмедиаплайер
description: Событие предупреждения зарезервировано для будущего использования.
ms.assetid: 3de63756-2726-4864-8988-fd614f23bcad
keywords:
- событие предупреждения объекта аксвиндовсмедиаплайер проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Warning Event of the AxWindowsMediaPlayer Object
api_location:
- AxInterop.WMPLib.dll
api_type:
- Assembly
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2a868ba7f619287cd96929c62d89dee3555d908b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243304"
---
# <a name="warning-event-of-the-axwindowsmediaplayer-object"></a>Событие Warning объекта Аксвиндовсмедиаплайер

Событие предупреждения зарезервировано для будущего использования.

``` syntax
[C#]
private void player_Warning(
  object sender,
  _WMPOCXEvents_WarningEvent e
)

[Visual Basic]
Private Sub player_Warning(
  sender As Object,
  e As _WMPOCXEvents_WarningEvent
) Handles player.Warning
```

## <a name="event-data"></a>Данные о событиях

Обработчик, связанный с этим событием, имеет тип **аксвмплиб. \_ Вмпокксевентс \_ варнинжевенсандлер**. Этот обработчик получает аргумент типа **аксвмплиб. \_ Вмпокксевентс \_ варнинжевент**, который содержит следующие свойства, связанные с этим событием.



| Свойство.    | Описание                                |
|-------------|--------------------------------------------|
| варнингтипе | **System. Int32** Не поддерживается.<br/>  |
| param       | **System. Int32** Не поддерживается.<br/>  |
| description | **System. String** Не поддерживается.<br/> |



 

## <a name="remarks"></a>Remarks

Это событие зарезервировано для будущего использования.

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

 

 





