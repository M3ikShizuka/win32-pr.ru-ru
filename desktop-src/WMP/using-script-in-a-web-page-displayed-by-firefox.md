---
title: Использование сценария на веб-странице, отображаемой Firefox
description: Использование сценария на веб-странице, отображаемой Firefox
ms.assetid: 0f1d21b1-1824-4ba9-9c0e-bd23ba847d9d
keywords:
- проигрыватель Windows Media, встраивание ActiveX элемента управления
- проигрыватель Windows Media объектная модель, встраивание ActiveX элемента управления
- объектная модель, встраивание элемента управления ActiveX
- проигрыватель Windows Media мобильный, внедренный элемент управления ActiveX
- проигрыватель Windows Media элемент управления ActiveX, внедрение
- проигрыватель Windows Media управление мобильными ActiveXми, внедрение
- элемент управления ActiveX, встраивание
- проигрыватель Windows Media элемент управления ActiveX, веб-страницы
- проигрыватель Windows Media мобильный ActiveX элемент управления, веб-страницы
- элемент управления ActiveX, веб-страницы
- проигрыватель Windows Media ActiveX элемента управления, пример сценария
- проигрыватель Windows Media управление мобильными ActiveXми, пример скрипта
- ActiveX элемент управления, пример сценария
- внедрение, веб-страницы
- Внедрение веб-страниц, пример сценария
- проигрыватель Windows Media, Firefox
- объектная модель проигрыватель Windows Media, Firefox
- Объектная модель, Firefox
- проигрыватель Windows Media Mobile, Firefox
- проигрыватель Windows Media ActiveX элемент управления, Firefox
- проигрыватель Windows Media мобильный ActiveX элемент управления, Firefox
- ActiveX элемент управления, Firefox
- Firefox, пример сценария
- Внедрение веб-страниц, Firefox
- Пример сценария для внедрения веб-страниц
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b8629f87f954d12602999f76483fdd36ab279290
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469630"
---
# <a name="using-script-in-a-web-page-displayed-by-firefox"></a>Использование сценария на веб-странице, отображаемой Firefox

Скрипт на веб-странице может использовать объектную модель проигрывателя для управления проигрывателем при взаимодействии пользователя со страницей. Например, следующий элемент INPUT содержит сценарий, который задает громкость проигрывателя.


```HTML
<INPUT type="button" value="Vol" OnClick="ChangeVolume()"/>
 
<SCRIPT>
  function ChangeVolume()
  {
    Player.settings.volume = 90;
  }
</SCRIPT>

```



многие объекты в объектной модели проигрыватель Windows Media поддерживаются Internet Explorer и подключаемым модулем Firefox. Тем не менее некоторые объекты не поддерживаются подключаемым модулем Firefox. В следующей таблице перечислены все объекты в объектной модели проигрывателя и показано, какие объекты поддерживаются подключаемым модулем Firefox.



| Объект                                              | Поддержка Firefox |
|-----------------------------------------------------|-----------------|
| [ROM](cdrom-object.md)                           | Нет              |
| [кдромколлектион](cdromcollection-object.md)       | Нет              |
| [клоседкаптион](closedcaption-object.md)           | Да             |
| [Элементы управления](controls-object.md)                     | Нет              |
| [ОПТИЧЕСКИ](dvd-object.md)                               | Нет              |
| [Ошибка](error-object.md)                           | Да             |
| [ерроритем](erroritem-object.md)                   | Да             |
| [Носитель](media-object.md)                           | Да             |
| [медиаколлектион](mediacollection-object.md)       | Нет              |
| [метадатапиктуре](metadatapicture-object.md)       | Нет              |
| [метадататекст](metadatatext-object.md)             | Нет              |
| [Network](network-object.md)                       | Да             |
| [Игрок](player-object.md)                         | Да             |
| [PlayerApplication](playerapplication-object.md)   | Нет              |
| [Список воспроизведения](playlist-object.md)                     | Да             |
| [плайлистаррай](playlistarray-object.md)           | Нет              |
| [плайлистколлектион](playlistcollection-object.md) | Нет              |
| [Запрос](query-object.md)                           | Нет              |
| [Параметры](settings-object.md)                     | Да             |
| [StringCollection](stringcollection-object.md)     | Нет              |



 

Подключаемый модуль Firefox поддерживает объект **Player** , но некоторые свойства объекта **Player** возвращают **значение NULL** в браузере Firefox. Например, свойство [кдромколлектион](player-cdromcollection.md) объекта **Player** возвращает **значение NULL** , так как подключаемый модуль Firefox не поддерживает объект **CDROM** . Аналогичным образом, свойства [DVD](player-dvd.md), [медиаколлектион](player-mediacollection.md), [плайераппликатион](player-playerapplication.md)и [плайлистколлектион](player-playlistcollection.md) объекта **Player** возвращают **значение NULL** в браузере Firefox.

Свойство **Player. плугинверсионинфо** поддерживается подключаемым модулем Firefox, но не Internet Explorer. Это свойство возвращает версию подключаемого модуля Firefox.

Подключаемый модуль Firefox поддерживает объект **мультимедиа** , включая свойство [жетитеминфобитипе](media-getiteminfobytype.md) . Однако в браузере Firefox свойство **жетитеминфобитипе** не поддерживает возвращаемые типы **метадататекст** и **метадатапиктуре** .

подключаемый модуль Firefox поддерживает объект [Параметры](settings-object.md) , за исключением метода [setMode](settings-setmode.md) и свойства [рекуестмедиаакцессригхтс](settings-requestmediaaccessrights.md) . В браузере Firefox свойство **рекуестмедиаакцессригхт** всегда возвращает значение false.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**использование элемента управления проигрыватель Windows Media с браузером Firefox**](using-the-windows-media-player-control-with-firefox.md)
</dt> </dl>

 

 




