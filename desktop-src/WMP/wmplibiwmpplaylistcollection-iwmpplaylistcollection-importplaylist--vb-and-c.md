---
title: Ивмпплайлистколлектион Импортплайлист, метод
description: Метод Импортплайлист добавляет статический список воспроизведения в библиотеку. | Ивмпплайлистколлектион Импортплайлист, метод
ms.assetid: 7a64e618-920d-419d-8769-612ab5dff49b
keywords:
- проигрыватель Windows Media метода импортплайлист
- проигрыватель Windows Media метода импортплайлист, интерфейс ивмпплайлистколлектион
- проигрыватель Windows Media интерфейса ивмпплайлистколлектион, метод импортплайлист
topic_type:
- apiref
api_name:
- IWMPPlaylistCollection.importPlaylist
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ad3ca727155d6ae859123d427812d93ebaa0b05c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459242"
---
# <a name="iwmpplaylistcollectionimportplaylist-method"></a>Метод Ивмпплайлистколлектион:: Импортплайлист

Метод **импортплайлист** добавляет статический список воспроизведения в библиотеку.

## <a name="syntax"></a>Синтаксис


```CSharp
public IWMPPlaylist importPlaylist(
  IWMPPlaylist pItem
);
```


```VB

Public Function importPlaylist( _
  ByVal pItem As IWMPPlaylist _
) As IWMPPlaylist
Implements IWMPPlaylistCollection.importPlaylist
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*питем* \[ окне\]
</dt> <dd>

Интерфейс **вмплиб. ивмпплайлист** для списка воспроизведения, который будет добавлен этим методом.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Интерфейс **вмплиб. ивмпплайлист** для добавленного списка воспроизведения.

## <a name="remarks"></a>Комментарии

Списки воспроизведения, которые не содержат элементов мультимедиа, не могут быть добавлены в библиотеку с помощью этого метода. Чтобы создать пустой список воспроизведения в библиотеке, используйте метод **невплайлист** . Затем можно заполнить итоговый список воспроизведения с помощью элементов мультимедиа, используя **ивмпплайлист. аппендитем** или **ивмпплайлист. insertItem**.

Если передать этот метод автоматическому списку воспроизведения, запрос выполняется один раз, а результат добавляется в библиотеку в виде статического списка воспроизведения. Чтобы добавить автоматический список воспроизведения в библиотеку и сохранить его автоматическое поведение, используйте **ивмпмедиаколлектион. Add**. Дополнительные сведения см. в разделе [статические и автоматические списки воспроизведения](static-and-auto-playlists.md).

Перед вызовом этого метода необходимо иметь доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                                                     |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Ивмпмедиаколлектион. Add (VB и C#)**](wmplibiwmpmediacollection-iwmpmediacollection-add--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлист (VB и C#)**](iwmpplaylist--vb-and-c.md)
</dt> <dt>

[**Ивмпплайлист. Аппендитем (VB и C#)**](wmplibiwmpplaylist-iwmpplaylist-appenditem--vb-and-c.md)
</dt> <dt>

[**Ивмпплайлист. insertItem (VB и C#)**](wmplibiwmpplaylist-iwmpplaylist-insertitem--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлистколлектион (VB и C#)**](iwmpplaylistcollection--vb-and-c.md)
</dt> <dt>

[**Ивмпплайлистколлектион. Невплайлист (VB и C#)**](wmplibiwmpplaylistcollection-iwmpplaylistcollection-newplaylist--vb-and-c.md)
</dt> </dl>

 

 





