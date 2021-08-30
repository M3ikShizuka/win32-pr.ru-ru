---
description: Фильтр модуля подготовки отчетов для команды внутреннего скрипта
ms.assetid: 264cc7c3-987c-4832-85a2-087278a4d024
title: Фильтр модуля подготовки отчетов для команды внутреннего скрипта
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 833c8b1034277019bfcaf222f78ab00a5c2cc8a8
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122478880"
---
# <a name="internal-script-command-renderer-filter"></a>Фильтр модуля подготовки отчетов для команды внутреннего скрипта

Получает команды сценария и отправляет их в приложение.

Этот фильтр принимает команды сценария в одном из двух форматов:

-   MEDIATYPE \_ Text: каждый пример носителя содержит текстовую строку ANSI.
-   MEDIATYPE \_ команду скрипта. Каждый пример носителя содержит две строки в Юникоде, заканчивающиеся нулем, сцепленные вместе. Первая строка описывает тип команды, а вторая — команду скрипта.

    Когда фильтр получает образец, он отправляет уведомление о событии [**EC \_ OLE \_**](ec-ole-event.md) . Первый параметр события — это **BSTR** с типом команды, или, `Text` Если используется формат MEDIATYPE \_ Text. Вторым параметром события является **BSTR** с командой скрипта. Приложение может получить событие и ответить на команду скрипта.

Пример использования этого фильтра см. в разделе [средство синтаксического анализа Sami (CC)](sami--cc--parser-filter.md).




| | | Интерфейсы фильтра | <a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>Ибасефилтер</strong></a>, <a href="/windows/desktop/api/Control/nn-control-imediaposition"><strong>имедиапоситион</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-imediaseeking"><strong>имедиасикинг</strong></a> | | Типы входных закрепления <ul><li>MEDIATYPE_ScriptCommand, MEDIASUBTYPE_NULL</li><li>MEDIATYPE_Text, MEDIASUBTYPE_NULL</li></ul> | | Интерфейсы входных закрепления | <a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"><strong>Имеминпутпин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>Ипин</strong></a>, <a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a> | | Типы выходных закрепления Неприменимо | | Интерфейсы выходного ПИН-кода | Неприменимо | | Фильтровать CLSID | {48025243-2D39-11CE-875D-00608CB78066} | | CLSID страницы свойств | Нет страницы свойств | | Исполняемый файл | Quartz.dll | | <a href="merit.md"></a> Кому | MERIT_PREFERRED + 1 | | <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 



