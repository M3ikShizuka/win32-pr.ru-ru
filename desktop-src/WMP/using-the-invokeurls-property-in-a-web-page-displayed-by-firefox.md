---
title: Использование свойства Инвокеурлс на веб-странице, отображаемой в браузере Firefox
description: Использование свойства Инвокеурлс на веб-странице, отображаемой в браузере Firefox
ms.assetid: cec2ba89-b08f-4c83-bcb2-a4df1ce6f179
keywords:
- проигрыватель Windows Media, встраивание ActiveX элемента управления
- проигрыватель Windows Media объектная модель, встраивание ActiveX элемента управления
- объектная модель, встраивание элемента управления ActiveX
- проигрыватель Windows Media мобильный, внедренный элемент управления ActiveX
- проигрыватель Windows Media элемент управления ActiveX, внедрение
- проигрыватель Windows Media управление мобильными ActiveXми, внедрение
- проигрыватель Windows Media элемент управления ActiveX, веб-страницы
- проигрыватель Windows Media мобильный ActiveX элемент управления, веб-страницы
- проигрыватель Windows Media элемент управления ActiveX, свойство инвокеурлс
- проигрыватель Windows Media элемент управления Mobile ActiveX, свойство инвокеурлс
- внедрение, веб-страницы
- Веб-страница внедрения, свойство Инвокеурлс
- проигрыватель Windows Media, Firefox
- объектная модель проигрыватель Windows Media, Firefox
- Объектная модель, Firefox
- проигрыватель Windows Media ActiveX элемент управления, Firefox
- ActiveX элемент управления, Firefox
- Firefox, свойство Инвокеурлс
- Внедрение веб-страниц, Firefox
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2487ebba1ff5664537dbaf0b0abad02a98acecf3c5985f1c09ffe9f8bbb743c2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118117113"
---
# <a name="using-the-invokeurls-property-in-a-web-page-displayed-by-firefox"></a>Использование свойства Инвокеурлс на веб-странице, отображаемой в браузере Firefox

некоторые файлы мультимедиа содержат внедренные url-адреса, для которых проигрыватель Windows Media отображает веб-страницы в окне или фрейме браузера по мере воспроизведения файла мультимедиа. в Windows Internet Explorer можно использовать свойство [Параметры. инвокеурлс](settings-invokeurls.md) , чтобы указать, отображаются ли страницы для внедренных url-адресов, а также можно использовать свойство [Параметры. дефаултфраме](settings-defaultframe.md) , чтобы указать кадр для отображения таких страниц.

В Firefox некоторые обходные пути необходимы для установки свойства **инвокеурлс** и для указания кадра для отображения страниц для внедренных URL-адресов.

## <a name="setting-the-invokeurls-property"></a>Установка свойства Инвокеурлс

значение свойства **Параметры. инвокеурлс** по умолчанию равно true, поэтому если требуется, чтобы значение было равно false, необходимо явно задать его. В Internet Explorer можно задать **инвокеурлс** в качестве значения false в элементе param внутри элемента объекта управления Player.

Подключаемый модуль Firefox не поддерживает задание свойства **инвокеурлс** в элементе param.

Это ограничение можно обойти, задав свойство **инвокеурлс** в скрипте. В следующем коде показано, как установить свойство **инвокеурлс** в значение false на веб-странице, которая может отображаться как в Internet Explorer, так и в браузере Firefox.


```HTML
<HTML>
  <BODY OnLoad="Initialize()">

    <SCRIPT type="text/javascript">

      document.write('<OBJECT id="Player"'); 

      if(-1 != navigator.userAgent.indexOf("MSIE"))
      {               
        document.write(' classid="clsid:6BF52A52-394A-11d3-B153-00C04F79FAA6"');       
      }
      else if(-1 != navigator.userAgent.indexOf("Firefox"))
      {      
        document.write(' type="application/x-ms-wmp"');        
      }  

      document.write(' width=300 height=200>');
      document.write('<PARAM name="autoStart" value="false"/>');
      document.write('<PARAM name="url" value="c:\\MediaFiles\\Glass.wmv"/>');
      document.write('</OBJECT>'); 
      
    </SCRIPT>

    <SCRIPT>
      function Initialize()
      {
        Player.settings.invokeURLs = false;
        Player.controls.play();
      }
    </SCRIPT>

  </BODY>
</HTML>

```



## <a name="displaying-webpages-in-a-frame"></a>Отображение веб-страниц в рамке

Файл мультимедиа может содержать URL-адреса, отображающие веб-страницы в окне или рамке браузера по мере воспроизведения файла мультимедиа. в Internet Explorer можно использовать свойство [Параметры. дефаултфраме](settings-defaultframe.md) , чтобы указать кадр, в котором отображаются эти страницы. Если не задать свойство **дефаултфраме** , URL-адреса будут отображаться в отдельном окне браузера по умолчанию. однако подключаемый модуль Firefox не поддерживает свойство **Параметры. дефаултфраме** . чтобы обойти это ограничение, присвойте свойству **Параметры. инвокеурлс** значение false и напишите обработчик событий [команду скрипта](player-player-scriptcommand.md) , который задает расположение целевого кадра. Этот метод показан в следующем примере, который работает в Internet Explorer и Firefox. Предположим, что веб-страница, показанная в примере, находится в кадрах \[ 0 \] , и вы хотите, чтобы страница URL-адреса отображалась в кадрах \[ 1 \] .


```HTML
<HTML>
  <BODY OnLoad="Initialize()">

    <SCRIPT type="text/javascript">

      document.write('<OBJECT id="Player"'); 

      if(-1 != navigator.userAgent.indexOf("MSIE"))
      {               
        document.write(' classid="clsid:6BF52A52-394A-11d3-B153-00C04F79FAA6"');       
      }
      else if(-1 != navigator.userAgent.indexOf("Firefox"))
      {      
        document.write(' type="application/x-ms-wmp"');        
      }  

      document.write(' width=300 height=200>');
      document.write('<PARAM name="autoStart" value="false"/>');
      document.write('<PARAM name="url" value="c:\\MediaFiles\\Glass.wmv"/>');
      document.write('</OBJECT>'); 
      
    </SCRIPT>

    <SCRIPT>
      function Initialize()
      {
        Player.settings.invokeURLs = false;
        Player.controls.play();
      }
    </SCRIPT>

    <SCRIPT for="Player" event="ScriptCommand(scType, scParam)">
      if( scType == "URL" )
      {
        parent.frames[1].location = scParam;
      }
    </script>

  </BODY>
</HTML>

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**использование элемента управления проигрыватель Windows Media с браузером Firefox**](using-the-windows-media-player-control-with-firefox.md)
</dt> </dl>

 

 




