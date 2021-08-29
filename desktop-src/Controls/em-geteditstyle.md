---
title: Сообщение EM_GETEDITSTYLE (RichEdit. h)
description: Извлекает текущие флаги изменения стиля.
ms.assetid: 568e51a4-0767-4a59-bf34-bc0281b5fe65
keywords:
- элементы управления Windows сообщений EM_GETEDITSTYLE
topic_type:
- apiref
api_name:
- EM_GETEDITSTYLE
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 220138a63628df310e316b6042045b7ca04ccbba
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122481590"
---
# <a name="em_geteditstyle-message"></a>\_Сообщение ЖЕТЕДИТСТИЛЕ EM

Извлекает текущие флаги изменения стиля.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает текущие флаги изменения стиля, которые могут включать одно или несколько из следующих значений:




| Код возврата | Описание | 
|-------------|-------------|
| <dl><dt><strong>SES_BEEPONMAXTEXT</strong></dt></dl> | Расширенное редактирование вызовет системный звуковой сигнал, если пользователь пытается ввести больше максимального числа символов.<br /> | 
| <dl><dt><strong>SES_BIDI</strong></dt></dl> | Включает двунаправленную обработку. Этот параметр автоматически включается с помощью расширенного редактирования, если доступны следующие стили окна: <a href="/windows/desktop/winmsg/extended-window-styles"><strong>WS_EX_RIGHT</strong></a>, <a href="/windows/desktop/winmsg/extended-window-styles"><strong>WS_EX_RTLREADING</strong></a>, <a href="/windows/desktop/winmsg/extended-window-styles"><strong>WS_EX_LEFTSCROLLBAR</strong></a>. Однако этот параметр полезен для обработки этих стилей окна при использовании пользовательской реализации <a href="/windows/desktop/api/Textserv/nl-textserv-itexthost"><strong>итекссост</strong></a> (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_CTFALLOWEMBED</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1</strong>): разрешить вставку внедренных объектов с помощью TSF (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_CTFALLOWPROOFING</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1</strong>): разрешает советы по проверке правописания TSF (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_CTFALLOWSMARTTAG</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1</strong>): разрешает советы SmartTag для TSF (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_CTFNOLOCK</strong></dt></dl> | <strong>Windows 8</strong>: не разрешать доступ на чтение и запись для блокировки TSF. Это приостанавливает ввод TSF. <br /> | 
| <dl><dt><strong>SES_DEFAULTLATINLIGA</strong></dt></dl> | <strong>Windows 8</strong>: шрифты с лигатурой типа "fi" отображаются с функциями OpenType по умолчанию, что приводит к улучшенному оформлению (по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_DRAFTMODE</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1)</strong>: используйте шрифты режима черновика для вывода текста. Режим черновика является параметром специальных возможностей, в котором элемент управления отображает текст с одним шрифтом. шрифт определяется параметром системы для шрифта, используемого в окнах сообщений. Например, доступные пользователи могут читать текст проще, если он является однородным, а не сочетанием шрифтов и стилей (значение по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_EMULATE10</strong></dt></dl> | <strong>Windows 8</strong>: эмуляция поведения RichEdit 1,0. <br /><blockquote>[!Note]<br />если вы действительно хотите это поведение, используйте Windows riched32.dll вместо riched20.dll или msftedit.dll. Riched32.dll имеет больше функциональных возможностей.</blockquote><br /> | 
| <dl><dt><strong>SES_EMULATESYSEDIT</strong></dt></dl> | Если этот бит включен, широкие возможности редактирования попытаются эмулировать элемент управления "изменение системы" (значение по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_EXTENDBACKCOLOR</strong></dt></dl> | Расширяет цвет фона до границ прямоугольника клиента (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_HIDEGRIDLINES</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1)</strong>: если ширина линий сетки таблицы равна нулю, линии сетки не отображаются. Это эквивалентно функции скрыть сетку в меню таблицы Word (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_HYPERLINKTOOLTIPS</strong></dt></dl> | <strong>Windows 8</strong>: когда курсор наведен на ссылку, отобразится всплывающая подсказка с адресом целевой ссылки (по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_LOGICALCARET</strong></dt></dl> | <strong>Windows 8</strong>: укажите логическую информацию о курсоре вместо точечного рисунка курсора, как описано в <a href="/windows/desktop/api/Textserv/nf-textserv-itexthost-txsetcaretpos"><strong>итекссост:: ткссеткаретпос</strong></a> (по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_LOWERCASE</strong></dt></dl> | Преобразует все входные символы в нижний регистр (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_MAPCPS</strong></dt></dl> | Является устаревшей. Не используйте.<br /> | 
| <dl><dt><strong>SES_MULTISELECT</strong></dt></dl> | <strong>Windows 8</strong>: включение множественного выбора с индивидуальным выбором мыши при нажатии клавиши Ctrl (значение по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_NOEALINEHEIGHTADJUST</strong></dt></dl> | <strong>Windows 8</strong>: не изменять высоту строки для восточно-азиатского текста (значение по умолчанию: 0, при котором высота линии изменяется на 15%). <br /> | 
| <dl><dt><strong>SES_NOFOCUSLINKNOTIFY</strong></dt></dl> | Отправляет <a href="en-link.md">EN_LINK</a> уведомления о ссылках, которые не имеют фокуса.<br /> | 
| <dl><dt><strong>SES_NOIME</strong></dt></dl> | Запрещает редакторы IME для данного экземпляра элемента управления Rich Edit (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_NOINPUTSEQUENCECHK</strong></dt></dl> | Если этот бит включен, то Расширенное редактирование не проверяет последовательность введенного текста. Для некоторых языков (например, тайского и вьетнамского) требуется проверка порядка входных последовательностей перед их отправкой в резервное хранилище (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_SCROLLONKILLFOCUS</strong></dt></dl> | Когда происходит Киллфокус, прокрутите до начала текста (позиции символа, равной 0) (значение по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_SMARTDRAGDROP</strong></dt></dl> | <strong>Windows 8</strong>: добавление или удаление пробела в соответствии с контекстом при перетаскивании текста (по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_USECRLF</strong></dt></dl> | Является устаревшей. Не используйте.<br /> | 
| <dl><dt><strong>SES_WORDDRAGDROP</strong></dt></dl> | <strong>Windows 8</strong>: если слово select активно, убедитесь, что расположение сброса находится на границе слова (по умолчанию: 0). <br /> | 
| <dl><dt><strong>SES_UPPERCASE</strong></dt></dl> | Преобразует все входные символы в верхний регистр (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_USEAIMM</strong></dt></dl> | Использует компонент активного входного метода IMM, поставляемый с Internet Explorer 4,0 или более поздней версии (по умолчанию: 0).<br /> | 
| <dl><dt><strong>SES_USEATFONT</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1)</strong>: использует шрифт @, предназначенный для вертикального текста; Он используется с стилем окна <a href="rich-edit-control-styles.md"><strong>ES_VERTICAL</strong></a> . Имя @ Font начинается с символа @, например " @Batang " (по умолчанию: 0, но автоматически включается для вертикального макета текста). <br /> | 
| <dl><dt><strong>SES_USECTF</strong></dt></dl> | <strong>Windows XP с пакетом обновления 1 (SP1)</strong>: включает поддержку TSF. (по умолчанию: 0)<br /> | 
| <dl><dt><strong>SES_XLTCRCRLFTOCR</strong></dt></dl> | Включает перевод Кркрлфс в CR. Если этот бит включен и файл считывается в, все экземпляры КРКРЛФ будут внутренне преобразованы в жесткие запросы CR. Это повлияет на перенос текста. Обратите внимание, что если такой файл сохраняется в виде обычного текста, запросы CR будут заменены символами CRLF. Это .txt стандарт для обычного текста (значение по умолчанию: 0, при котором удаляется Кркрлфс на входе). <br /> | 




 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Распространяемые компоненты<br/>          | Расширенное редактирование 3,0<br/>                                                              |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**EM \_ сетедитстиле**](em-seteditstyle.md)
</dt> </dl>

 

