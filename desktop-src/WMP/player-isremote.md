---
title: Player. Remote
description: свойство "remote" извлекает значение, указывающее, выполняется ли элемент управления проигрыватель Windows Media в удаленном режиме.
ms.assetid: bfeab968-affb-4d5d-b88b-5caf50d34cee
keywords:
- Player. remote проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Player.isRemote
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b7c8d97ba212e032db16b43299d2a3a8a836f9b9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172748"
---
# <a name="playerisremote"></a>Player. Remote

свойство " **remote** " извлекает значение, указывающее, выполняется ли элемент управления проигрыватель Windows Media в удаленном режиме.

## <a name="syntax"></a>Синтаксис

*проигрыватель* . **Удаленный**

## <a name="possible-values"></a>Возможные значения

Это свойство является **логическим значением**, доступным только для чтения.



| Значение | Описание                                   |
|-------|-----------------------------------------------|
| Да  | Элемент управления "проигрыватель" работает в удаленном режиме. |
| false | Элемент управления "проигрыватель" выполняется в локальном режиме.  |



 

## <a name="remarks"></a>Remarks

**проигрыватель Windows Media 10 Mobile:** Это свойство всегда возвращает значение false.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> <dt>

[**Реализация удаленного управления проигрывателем Windows Media**](remoting-the-windows-media-player-control.md)
</dt> </dl>

 

 





