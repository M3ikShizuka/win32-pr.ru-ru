---
title: Аксвиндовсмедиаплайер. Опенстате, свойство
description: Свойство Опенстате возвращает значение перечисления, указывающее состояние источника содержимого.
ms.assetid: 7a76814a-649f-4516-a92a-5f536fb1b147
keywords:
- проигрыватель Windows Media свойства опенстате
- проигрыватель Windows Media свойства опенстате, класс аксвиндовсмедиаплайер
- проигрыватель Windows Media класса аксвиндовсмедиаплайер, свойство опенстате
topic_type:
- apiref
api_name:
- AxWindowsMediaPlayer.openState
api_location:
- AxInterop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 919bf906ce67793c4cd26f32892eae8acf441295
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126889680"
---
# <a name="axwindowsmediaplayeropenstate-property"></a>Аксвиндовсмедиаплайер. Опенстате, свойство

Свойство Опенстате возвращает значение перечисления, указывающее состояние источника содержимого.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```CSharp
public WMPOpenState openState {get;}
```


```VB

Public ReadOnly Property openState As WMPOpenState
```





## <a name="property-value"></a>Значение свойства

Значение перечисления Вмплиб. Вмпопенстате.

## <a name="remarks"></a>Комментарии

состояния проигрыватель Windows Media не гарантированно выполняются в каком бы то ни было определенном порядке. Кроме того, не все состояния должны происходить во время последовательности событий. Не следует писать код, зависящий от порядка состояний.

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

[**Аксвиндовсмедиаплайер. Опенстатечанже, событие**](axwmplib-axwindowsmediaplayer-openstatechange.md)
</dt> <dt>

[**Вмплиб. Вмпопенстате**](/previous-versions/windows/desktop/api/wmp/ne-wmp-wmpopenstate)
</dt> </dl>

 

 





