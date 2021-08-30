---
description: Работа с эффектами и переходами
ms.assetid: 00e97d02-ff43-4e1f-9806-abaeb9288058
title: Работа с эффектами и переходами
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7503ffd929689e0c53ac2c273faf0a635fc581ee540acf03e8db6ea9647a1912
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119982184"
---
# <a name="working-with-effects-and-transitions"></a>Работа с эффектами и переходами

\[Этот API не поддерживается и может быть изменен или недоступен в будущем.\]

Эффекты изменяют один клип, запись или композицию. Переходы создают секуес из одной или компоситионсто другой.

[DirectShow службы редактирования](directshow-editing-services.md) используют объекты преобразования DirectX для воспроизведения видео и видеоэффектов. Для видеопереходов используйте любой двухмерный входной объект преобразования DirectX. Для видеоэффектов используйте любой трехмерный один входной объект преобразования DirectX. Корпорация Майкрософт больше не поддерживает разработку объектов преобразования DirectX сторонних производителей. однако некоторые из них предоставляются с помощью DirectShow, а другие предоставляются в Microsoft Internet Explorer. Дополнительные сведения о переходах, предоставляемых в Internet Explorer, см. в разделе [Справочник по визуальным фильтрам и переходам](/previous-versions/windows/internet-explorer/ie-developer/platform-apis/ms532853(v=vs.85)).

для звуковых эффектов можно использовать любой DirectShow фильтр звукового эффекта. DES также предоставляет [эффекты конверта тома](volume-envelope-effect.md) для настройки тома на дорожке или клипе. DES не поддерживает смену звука.

В этом разделе рассматриваются следующие вопросы.

-   [Добавление эффектов и объектов перехода](adding-effect-and-transition-objects.md)
-   [Предварительный просмотр эффектов и переходов](previewing-effects-and-transitions.md)
-   [Перечисление эффектов и переходов](enumerating-effects-and-transitions.md)
-   [Задание свойств для эффектов и переходов](setting-properties-on-effects-and-transitions.md)
-   [Направление перехода](transition-direction.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[использование служб DirectShow editing Services](using-directshow-editing-services.md)
</dt> </dl>

 

 
