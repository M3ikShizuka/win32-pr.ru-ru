---
title: Ссылки на обложки в URL-адресах
description: Ссылки на обложки в URL-адресах
ms.assetid: 9ae30c12-2dee-46b2-90e2-c101a83856fb
keywords:
- обложки проигрыватель Windows Media, URL-ссылки
- обложки, URL-ссылки
- URL-ссылки в обложках
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 75b33ac9a5f37dce242797ae93dc4e85b973c76b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127581334"
---
# <a name="referencing-skins-in-urls"></a>Ссылки на обложки в URL-адресах

при использовании URL-адреса для загрузки файла мультимедиа, который будет воспроизводиться проигрыватель Windows Media, можно запросить использование определенной обложки с этим файлом. Если обложка уже установлена на компьютере пользователя, она будет использоваться. в противном случае будет использоваться Предыдущая обложка.

Чтобы запросить обложку, добавьте в конец URL-адреса следующее:


```C++
?WMPSkin=skinname
```



*скиннаме* — имя обложки, которую необходимо запросить. Не используйте кавычки вокруг имени обложки.

Например, чтобы запросить использование обложки хеадспаце, введите следующий URL-адрес http:


```C++
https://www.proseware.com/mymedia.wma?WMPSkin=headspace

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**О обложках**](about-skins.md)
</dt> </dl>

 

 




