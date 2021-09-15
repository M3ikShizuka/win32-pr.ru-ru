---
title: Ивмпплайлистколлектион Жеталл, метод
description: Метод Жеталл возвращает интерфейс Ивмпплайлистаррай, который предоставляет доступ ко всем спискам воспроизведения в библиотеке.
ms.assetid: d36dbc5c-ccb0-400a-ab5b-918598c218f1
keywords:
- проигрыватель Windows Media метода жеталл
- проигрыватель Windows Media метода жеталл, интерфейс ивмпплайлистколлектион
- проигрыватель Windows Media интерфейса ивмпплайлистколлектион, метод жеталл
topic_type:
- apiref
api_name:
- IWMPPlaylistCollection.getAll
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a4260f5c960650cf6c04a1dd8b39d887f711fb8a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459247"
---
# <a name="iwmpplaylistcollectiongetall-method"></a>Метод Ивмпплайлистколлектион:: Жеталл

Метод **жеталл** возвращает интерфейс **ивмпплайлистаррай** , который предоставляет доступ ко всем спискам воспроизведения в библиотеке.

## <a name="syntax"></a>Синтаксис


```CSharp
public IWMPPlaylistArray getAll();
```


```VB

Public Function getAll() As IWMPPlaylistArray
Implements IWMPPlaylistCollection.getAll
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Интерфейс **вмплиб. ивмпплайлистаррай** для извлеченного массива списков воспроизведения.

## <a name="remarks"></a>Комментарии

Перед вызовом этого метода необходимо иметь доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                                                     |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпплайлистаррай (VB и C#)**](iwmpplaylistarray--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлистколлектион (VB и C#)**](iwmpplaylistcollection--vb-and-c.md)
</dt> </dl>

 

 





