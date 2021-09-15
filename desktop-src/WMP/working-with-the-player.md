---
title: Работа с проигрывателем
description: Работа с проигрывателем
ms.assetid: 27aff735-2142-4506-b9d0-2c0fbe60fd6b
keywords:
- проигрыватель Windows Media обложки, атрибут игрока в JScript
- обложки, атрибут Player в JScript
- атрибуты, проигрыватель
- атрибут Player
- JScript файлы для обложек, атрибут player
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0d47ea74b4c91f92ef33106e40e9896b98de6a34
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459580"
---
# <a name="working-with-the-player"></a>Работа с проигрывателем

при использовании JScript майкрософт для доступа к методам и свойствам проигрыватель Windows Media необходимо использовать имя "Player" в качестве имени элемента управления. Например, для ссылки на метод останавливаться необходимо ввести:


```C++
player.Controls.Stop()

```



глобальный атрибут **игрока** — это ключ к доступу к элементу управления проигрыватель Windows Media через скрипты обложек. с помощью этого атрибута все объекты элемента управления проигрыватель Windows Media становятся доступными для изменения во время выполнения через их свойства и методы. Кроме того, доступен элемент **Player** , позволяющий задавать обработчики событий и атрибут **URL-адреса** во время разработки.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**Использование JScript**](using-jscript.md)
</dt> </dl>

 

 




