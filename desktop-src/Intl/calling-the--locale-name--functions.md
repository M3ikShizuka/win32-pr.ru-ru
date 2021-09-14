---
description: Windows В Vista введено большое количество функций, которые используют имена языковых стандартов вместо идентификаторов языкового стандарта.
ms.assetid: e88c31b2-b1da-40ae-b512-67b8ad409b95
title: Вызов функций "locale Name"
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c58c15d2d9fe7721eb162f8c7cf96084bd4afa2e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127274816"
---
# <a name="calling-the-locale-name-functions"></a>Вызов функций "locale Name"

Windows В Vista введено большое количество функций, которые используют [имена языковых](locale-names.md) стандартов вместо [идентификаторов языкового стандарта](locale-identifiers.md). Эти новые функции обеспечивают хорошую поддержку дополнительных [языковых стандартов](custom-locales.md), и некоторые из них предоставляют дополнительные функции, недоступные в старых функциях NLS. Некоторые из них, такие как новые функции перечисления, также представляют улучшения проектирования.

> [!Note]  
> приложения, предназначенные для работы только в Windows Vista и более поздних версиях, должны использовать функции "locale name" в предпочтениях к функциям NLS, использующим идентификаторы языкового стандарта.

 

В следующей таблице перечислены функции имени языкового стандарта и более старые функции, которые они могут заменить.



| Функции, использующие имена языковых стандартов                                     | Функции, использующие идентификаторы языковых стандартов                                                             |
|------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
| [**компарестринжекс**](/windows/desktop/api/Stringapiset/nf-stringapiset-comparestringex)                       | [**CompareString**](/windows/win32/api/stringapiset/nf-stringapiset-comparestringw)                                                         |
| [**енумкалендаринфоексекс**](/windows/desktop/api/Winnls/nf-winnls-enumcalendarinfoexex)             | [**Енумкалендаринфо**](/windows/desktop/api/Winnls/nf-winnls-enumcalendarinfoa), [ **енумкалендаринфоекс**](/windows/desktop/api/Winnls/nf-winnls-enumcalendarinfoexa) |
| [**енумдатеформатсексекс**](/windows/desktop/api/Winnls/nf-winnls-enumdateformatsexex)               | [**Енумдатеформатс**](/windows/desktop/api/Winnls/nf-winnls-enumdateformatsa), [ **енумдатеформатсекс**](/windows/desktop/api/Winnls/nf-winnls-enumdateformatsexa)     |
| [**енумсистемлокалесекс**](/windows/desktop/api/Winnls/nf-winnls-enumsystemlocalesex)               | [**енумсистемлокалес**](/windows/desktop/api/Winnls/nf-winnls-enumsystemlocalesa)                                                 |
| [**енумтимеформатсекс**](/windows/desktop/api/Winnls/nf-winnls-enumtimeformatsex)                   | [**енумтимеформатс**](/windows/desktop/api/Winnls/nf-winnls-enumtimeformatsa)                                                     |
| [**финднлсстринжекс**](/windows/desktop/api/Winnls/nf-winnls-findnlsstringex)                       | [**финднлсстринг**](/windows/desktop/api/Winnls/nf-winnls-findnlsstring)                                                         |
| [**жеткалендаринфоекс**](/windows/desktop/api/Winnls/nf-winnls-getcalendarinfoex)                   | [**жеткалендаринфо**](/windows/desktop/api/Winnls/nf-winnls-getcalendarinfoa)                                                     |
| [**жеткурренциформатекс**](/windows/desktop/api/Winnls/nf-winnls-getcurrencyformatex)               | [**жеткурренциформат**](/windows/desktop/api/Winnls/nf-winnls-getcurrencyformata)                                                 |
| [**жетдатеформатекс**](/windows/desktop/api/datetimeapi/nf-datetimeapi-getdateformatex)                       | [**жетдатеформат**](/windows/desktop/api/datetimeapi/nf-datetimeapi-getdateformata)                                                         |
| [**жетдуратионформатекс**](/windows/desktop/api/Winnls/nf-winnls-getdurationformatex)               | [**жетдуратионформат**](/windows/desktop/api/Winnls/nf-winnls-getdurationformat)                                                 |
| [**GetLocaleInfoEx**](/windows/desktop/api/Winnls/nf-winnls-getlocaleinfoex)                       | [**GetLocaleInfo**](/windows/desktop/api/Winnls/nf-winnls-getlocaleinfoa)                                                         |
| [**жетнлсверсионекс**](/windows/desktop/api/Winnls/nf-winnls-getnlsversionex)                       | [**жетнлсверсион**](/windows/desktop/api/Winnls/nf-winnls-getnlsversion)                                                         |
| [**жетнумберформатекс**](/windows/desktop/api/Winnls/nf-winnls-getnumberformatex)                   | [**жетнумберформат**](/windows/desktop/api/Winnls/nf-winnls-getnumberformata)                                                     |
| [**жетсистемдефаултлокаленаме**](/windows/desktop/api/Winnls/nf-winnls-getsystemdefaultlocalename) | [**жетсистемдефаултлЦид**](/windows/desktop/api/Winnls/nf-winnls-getsystemdefaultlcid)                                           |
| [**жеттимеформатекс**](/windows/desktop/api/datetimeapi/nf-datetimeapi-gettimeformatex)                       | [**жеттимеформат**](/windows/desktop/api/datetimeapi/nf-datetimeapi-gettimeformata)                                                         |
| [**жетусердефаултлокаленаме**](/windows/desktop/api/Winnls/nf-winnls-getuserdefaultlocalename)     | [**жетусердефаултлЦид**](/windows/desktop/api/Winnls/nf-winnls-getuserdefaultlcid)                                               |
| [**исвалидлокаленаме**](/windows/desktop/api/Winnls/nf-winnls-isvalidlocalename)                   | [**исвалидлокале**](/windows/desktop/api/Winnls/nf-winnls-isvalidlocale)                                                         |
| [**лкмапстринжекс**](/windows/desktop/api/Winnls/nf-winnls-lcmapstringex)                           | [**LCMapString завершилось ошибкой**](/windows/desktop/api/Winnls/nf-winnls-lcmapstringa)                                                             |



 

## <a name="example"></a>Пример

Пример, демонстрирующий использование нескольких функций на основе имен языковых стандартов, можно найти в [NLS: пример интерфейсов API на основе имен](nls--name-based-apis-sample.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Поддержка национальных языков](using-national-language-support.md)
</dt> </dl>

 

 
