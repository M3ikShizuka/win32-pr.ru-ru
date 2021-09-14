---
title: Метод CDROM. EJECT
description: Метод Eject извлекает компакт-диск или DVD-диск из накопителя. | Метод CDROM. EJECT
ms.assetid: f43c7f10-7de2-488c-833a-ecd3ac21744b
keywords:
- проигрыватель Windows Media метода извлечения
- метод извлечения проигрыватель Windows Media, класс Cdrom
- класс Cdrom проигрыватель Windows Media, метод извлечения
topic_type:
- apiref
api_name:
- Cdrom.eject
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 78326ca57dcf097344fc073681fae772222ea9ad
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242557"
---
# <a name="cdromeject-method"></a>Метод CDROM. EJECT

Метод **Eject** извлекает компакт-диск или DVD-диск из накопителя.

## <a name="syntax"></a>Синтаксис


```JScript
Cdrom.eject()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Если дверца диска открыта, этот метод закрывает дверцу.

Чтобы использовать этот метод, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

**проигрыватель Windows Media 10 Mobile:** Этот метод не поддерживается.

## <a name="examples"></a>Примеры

В следующем примере создается HTML-элемент Button, который использует *CDROM*. **Извлеките** , чтобы открыть дверцу диска с нулевым индексом описателя. Объект **Player** создан с идентификатором "Player".


```JScript
<INPUT TYPE = "BUTTON"
       NAME = "EJECTBUTTON"
       VALUE = "EJECT"
       OnClick =  "Player.cdromCollection.item(0).eject()"
>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Версия<br/>                  | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>                      | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект CDROM**](cdrom-object.md)
</dt> <dt>

[**Player. Плайстате**](player-playstate.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





