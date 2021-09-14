---
title: Метод списка воспроизведения. Сетитеминфо
description: Метод Сетитеминфо задает значение атрибута списка воспроизведения.
ms.assetid: ffecb43f-343d-4a4f-9356-0e3cfa85ce77
keywords:
- проигрыватель Windows Media метода сетитеминфо
- проигрыватель Windows Media метода сетитеминфо, класс списка воспроизведения
- класс списка воспроизведения проигрыватель Windows Media, метод сетитеминфо
topic_type:
- apiref
api_name:
- Playlist.setItemInfo
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8ff42e56e549100044db0881bb38ade5f2f1711a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343206"
---
# <a name="playlistsetiteminfo-method"></a>Метод списка воспроизведения. Сетитеминфо

Метод **сетитеминфо** задает значение атрибута списка воспроизведения.

## <a name="syntax"></a>Синтаксис


```JScript
Playlist.setItemInfo(
  name,
  value
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*имя* \[ окне\]
</dt> <dd>

**Строка** , содержащая имя атрибута, который необходимо задать. дополнительные сведения об атрибутах, поддерживаемых проигрыватель Windows Media, см. в [справочнике по атрибуту](attribute-reference.md)проигрыватель Windows Media.

</dd> <dt>

*значение* \[ окне\]
</dt> <dd>

**Строка** , содержащая новое значение атрибута.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Особое использование метода **сетитеминфо** заключается в сортировке элементов списка воспроизведения с помощью атрибута SortAttribute. в следующем примере JScript список воспроизведения сортируется по значениям атрибута усерластплайедтиме. Список воспроизведения переменных является ссылкой на объект **списка воспроизведения** .


```JScript
playlist.setItemInfo("SortAttribute", "UserLastPlayedTime")
```



Чтобы использовать этот метод, требуется полный доступ к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

**проигрыватель Windows Media 10 Mobile:** Этот метод не поддерживается.

## <a name="examples"></a>Примеры

Пример кода, в котором используется это свойство, см. в свойстве [аттрибутекаунт](playlist-attributecount.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект списка воспроизведения**](playlist-object.md)
</dt> <dt>

[**Список воспроизведения. getItemInfo**](playlist-getiteminfo.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





