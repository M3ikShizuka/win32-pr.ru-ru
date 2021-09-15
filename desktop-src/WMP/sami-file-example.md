---
title: Пример файла SAMI
description: Пример файла SAMI
ms.assetid: 52b566f1-0d87-4bf2-87b3-3821e69a5699
keywords:
- проигрыватель Windows Media, синхронизированный доступный медиа-обмен (SAMI)
- объектная модель проигрыватель Windows Media, синхронизированный доступный медиа-обмен (SAMI)
- Объектная модель, синхронизированный доступный медиа-обмен (SAMI)
- проигрыватель Windows Media Мобильный, синхронизированный доступный мультимедийный обмен (SAMI)
- проигрыватель Windows Media ActiveX элемент управления, синхронизированный доступный медиа-обмен (SAMI)
- проигрыватель Windows Media мобильный ActiveX элемент управления, синхронизированный доступный мультимедийный обмен (SAMI)
- ActiveX элемент управления, синхронизированный доступный медиа-обмен (SAMI)
- Синхронизированный доступный мультимедийный обмен (SAMI), файлы
- SAMI (синхронизированный доступный медиа-обмен), файлы
- Синхронизированный доступный мультимедийный обмен (SAMI), пример кода
- SAMId (синхронизированный доступный медиа-обмен), пример кода
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f9634de52f71b4ca1db151bdf9104c3891c8ce5d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469636"
---
# <a name="sami-file-example"></a>Пример файла SAMI

Следующий пример кода представляет собой полный файл SAMI с одним набором скрытых текста заголовка и несколькими объявлениями классов для стиля текста и языка описания.


```C++
<SAMI>
<HEAD>
   <STYLE TYPE = "text/css">
   <!--
   /* P defines the basic style selector for closed caption paragraph text */
   P {font-family:sans-serif; color:white;}
   /* Source, Small, and Big define additional ID selectors for closed caption text */
   #Source {color: orange; font-family: arial; font-size: 12pt;}
   #Small {Name: SmallTxt; font-size: 8pt; color: yellow;}
   #Big {Name: BigTxt; font-size: 12pt; color: magenta;}
   /* ENUSCC and FRFRCC define language class selectors for closed caption text */
   .ENUSCC {Name: 'English Captions'; lang: en-US; SAMIType: CC;}
   .FRFRCC {Name: 'French Captions'; lang: fr-FR; SAMIType: CC;}
   -->
   </STYLE>
</HEAD>
<BODY>
   <!<entity type="mdash"/>- The closed caption text displays at 1000 milliseconds. -->
   <SYNC Start = 1000>
      <!-- English closed captions -->
      <P Class = ENUSCC ID = Source>Narrator
      <P Class = ENUSCC>Great reason to visit Seattle, brought to you by two out-of-staters.
      <!-- French closed captions -->
      <P Class = FRFRCC ID = Source>Narrateur
      <P Class = FRFRCC>Deux personnes ne venant la r&eacute;gion vous donnent de bonnes raisons de visiter Seattle.
</BODY>
</SAMI>

```



Стили, определенные в файле SAMI, соответствуют стандартному синтаксису селектора CSS для элементов, классов и идентификаторов. В элементе BODY все элементы P имеют стиль, определенный для селектора элемента P в элементе STYLE. Атрибут Class элемента определяет язык элемента, определенный селекторами классов в элементе STYLE (селекторы, начинающиеся с точек). Имена языков, заданные селекторами класса, могут быть любой строкой. Для элементов с указанным атрибутом ID применяются дополнительные стили, как указано селекторами ИДЕНТИФИКАТОРов в элементе STYLE (селекторы начинаются с \# символов).

при использовании в сочетании с объектной моделью проигрыватель Windows Media селекторы классов соответствуют *клоседкаптион*. Свойство **самиланг** , которое можно использовать для указания языка заголовков. Селекторы ИДЕНТИФИКАТОРов соответствуют *клоседкаптион*. Свойство **самистиле** , которое можно использовать для указания стиля, в котором будут отображаться заголовки.

Дополнительные сведения о создании файлов SAMI см. в статье об использовании SAMI 1,0 на [веб-сайте Майкрософт](/documentation/).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Добавление субтитров к цифровым носителям**](adding-closed-captions-to-digital-media.md)
</dt> </dl>

 

 