---
title: Схема сообщений
description: Схема сообщений
ms.assetid: 4640b0f5-625e-4a9e-86f5-3e75d0afb40d
keywords:
- подключаемые модули проигрыватель Windows Media, схема сообщений
- подключаемые модули, схема сообщений
- подключаемые модули пользовательского интерфейса, схема сообщений
- Подключаемые модули пользовательского интерфейса, схема сообщений
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6ea7fc04caf752383368ab6e51ae19c82e8c3515
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168608"
---
# <a name="the-message-map"></a>Схема сообщений

Окно подключаемого модуля реагирует на различные события, вызывая методы, сопоставленные с соответствующими сообщениями о событиях. Мастер обеспечивает сопоставление таким образом, что onpain и Онерасебаккграунд будут вызываться в нужное время. Чтобы создать кнопку **поиска** и ответить на ее щелчки, раздел схемы сообщений изменяется следующим образом:


```C++
BEGIN_MSG_MAP(CPluginWindow)
    MESSAGE_HANDLER(WM_PAINT, OnPaint)
    MESSAGE_HANDLER(WM_ERASEBKGND, OnEraseBackground)
    MESSAGE_HANDLER(WM_CREATE, OnCreate)
    COMMAND_ID_HANDLER(IDC_SEARCH, OnSearch)
END_MSG_MAP()

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Реализация Кплугинвиндов**](implementing-cpluginwindow.md)
</dt> </dl>

 

 




