---
title: Аксвиндовсмедиаплайер. Невплайлист, метод
description: Метод Невплайлист возвращает интерфейс Ивмпплайлист для нового списка воспроизведения.
ms.assetid: caee8ee5-6201-474d-a4cb-80e574f84f0b
keywords:
- проигрыватель Windows Media метода невплайлист
- проигрыватель Windows Media метода невплайлист, класс аксвиндовсмедиаплайер
- класс аксвиндовсмедиаплайер проигрыватель Windows Media, метод невплайлист
topic_type:
- apiref
api_name:
- AxWindowsMediaPlayer.newPlaylist
api_location:
- AxInterop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f35bbc1d1c8a0f1f76d685676e08119b659ad119176036ab377f9525ce1ab0e7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120123894"
---
# <a name="axwindowsmediaplayernewplaylist-method"></a>Аксвиндовсмедиаплайер. Невплайлист, метод

Метод Невплайлист возвращает интерфейс Ивмпплайлист для нового списка воспроизведения.

## <a name="syntax"></a>Синтаксис


```CSharp
public IWMPPlaylist newPlaylist(
  System.String bstrName,
  System.String bstrURL
);
```


```VB

Public Function newPlaylist( _
  ByVal bstrName As System.String, _
  ByVal bstrURL As System.String _
) As IWMPPlaylist
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*bstrName* 
</dt> <dd>

**Строка System. String** , которая является именем нового списка воспроизведения.

</dd> <dt>

*бструрл* 
</dt> <dd>

**строка System. String** , которая является URL-адресом списка воспроизведения Windows Media metafile, используемого для инициализации нового списка воспроизведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Интерфейс Вмплиб. Ивмпплайлист, представляющий только что созданный список воспроизведения.

## <a name="remarks"></a>Remarks

Если параметр *бструрл* имеет значение null или является строкой нулевой длины (""), этот метод создает пустой **список воспроизведения**. Если параметр *bstrName* является строкой нулевой длины (""), этот метод применяет текущее имя метафайла.

Новый список воспроизведения, созданный с помощью этого метода, не добавляется в библиотеку. Чтобы добавить новый список воспроизведения в библиотеку, используйте Ивмпплайлистколлектион. **импортплайлист** или ивмпплайлистколлектион. **невплайлист**. Все начальные и конечные пробелы в имени списка воспроизведения автоматически удаляются при добавлении в библиотеку.

Так как библиотека допускает наличие нескольких списков воспроизведения с одинаковыми именами, перед добавлением нового списка воспроизведения может потребоваться проверить, есть ли у него указанное имя.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|----------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                          |
| Пространство имен<br/> | **аксвмплиб**<br/>                                                                                                    |
| Сборка<br/>  | <dl> <dt>AxInterop.WMPLib.dll (AxInterop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Аксвиндовсмедиаплайер (VB и C#)**](axwindowsmediaplayer-object--vb-and-c.md)
</dt> <dt>

[**Интерфейс Ивмпплайлист (VB и C#)**](iwmpplaylist--vb-and-c.md)
</dt> <dt>

[**Ивмпплайлистколлектион. Импортплайлист (VB и C#)**](wmplibiwmpplaylistcollection-iwmpplaylistcollection-importplaylist--vb-and-c.md)
</dt> <dt>

[**Ивмпплайлистколлектион. Невплайлист (VB и C#)**](wmplibiwmpplaylistcollection-iwmpplaylistcollection-newplaylist--vb-and-c.md)
</dt> </dl>

 

 





