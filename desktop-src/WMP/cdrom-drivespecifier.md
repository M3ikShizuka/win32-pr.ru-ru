---
title: CDROM. ДривеспеЦифиер
description: Свойство ДривеспеЦифиер извлекает букву CD или DVD-дисковода.
ms.assetid: f592819e-61ba-4ae1-b748-b6f29df88067
keywords:
- проигрыватель Windows Media Cdrom. дривеспеЦифиер
topic_type:
- apiref
api_name:
- Cdrom.driveSpecifier
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8a358e54dabf9186dba3a2eb56f38d6fa846aab92f0a8cab6347f568788a1ae5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119864194"
---
# <a name="cdromdrivespecifier"></a>CDROM. ДривеспеЦифиер

Свойство **дривеспеЦифиер** извлекает букву CD или DVD-дисковода.

``` syntax
player.cdromCollection.item(
        index
        ).driveSpecifier
      
```

## <a name="possible-values"></a>Возможные значения

Это свойство является **строкой**, доступная только для чтения.

## <a name="remarks"></a>Remarks

Обычно дисководы DVD могут воспроизводить компакт-диски, но дисководы компакт-дисков не могут воспроизводить DVD-носители. Это свойство получает описатель диска для индекса диска, начинающегося с нуля, в диапазоне, полученном с помощью *кдромколлектион*. **количество**. Полученное значение имеет вид *x*:, где *X* представляет букву диска.

Чтобы получить значение этого свойства, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

**проигрыватель Windows Media 10 Mobile:** Это свойство не поддерживается.

## <a name="examples"></a>Примеры

в следующем примере JScript используется *Cdrom*. **дривеспеЦифиер** для заполнения текстовой области HTML с именем myText с разделенным запятыми списком доступных ДИСКОВОДов компакт-и DVD-дисков. Объект **Player** создан с идентификатором "Player".


```JScript
// Allocate an array to store the drive specifiers.
var MYdriveSpecifiers = new Array();

// Loop through the available drives using CdromCollection.count.
for (var i = 0; i < Player.cdRomCollection.count; i++){

// For each available drive, add a corresponding item 
// to the MYdriveSpecifiers array. 
    MYdriveSpecifiers[i] = Player.CDRomCollection.item(i).driveSpecifier;
}

// Write the array of drive letter specifiers to the text area.
myText.value = "Drive letters found: " + MYdriveSpecifiers;
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Версия<br/>                  | проигрыватель Windows Media версии 7,0 или более поздней<br/>                               |
| DLL<br/>                      | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект CDROM**](cdrom-object.md)
</dt> <dt>

[**Кдромколлектион. Count**](cdromcollection-count.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





