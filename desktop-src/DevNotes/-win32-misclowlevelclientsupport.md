---
description: в этом разделе содержатся сведения о низкоуровневых api-интерфейсах, используемых клиентской инфраструктурой Windows.
ms.assetid: 14a6e970-2032-420e-9930-a15909dbbb97
title: Поддержка прочих Low-Level клиентов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5ffc5d32588089d3300ef59af17fe7ce2a0d0e99
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122470181"
---
# <a name="miscellaneous-low-level-client-support"></a>Поддержка прочих Low-Level клиентов

в этом разделе содержатся сведения о низкоуровневых api-интерфейсах, используемых клиентской инфраструктурой Windows.

### <a name="functions"></a>Функции




| Раздел | Содержимое | 
|-------|----------|
| <a href="/windows/desktop/api/winbase/nf-winbase-_lclose"><strong>_lclose</strong></a> | Функция _lclose закрывает указанный файл, чтобы он больше не был доступен для чтения или записи. Эта функция обеспечивает совместимость с 16-разрядными версиями Windows. Приложения на основе Win32 должны использовать функцию CloseHandle.<br /> | 
| <a href="/windows/desktop/api/winbase/nf-winbase-_lopen"><strong>_lopen</strong></a> | Функция _lopen открывает существующий файл и устанавливает указатель файла на начало файла. Эта функция обеспечивает совместимость с 16-разрядными версиями Windows. Приложения на основе Win32 должны использовать функцию CreateFile. <br /> | 
| <a href="/windows/desktop/api/winbase/nf-winbase-_lread"><strong>_lread</strong></a> | Функция _lread считывает данные из указанного файла. Эта функция обеспечивает совместимость с 16-разрядными версиями Windows. Приложения на основе Win32 должны использовать функцию ReadFile. <br /> | 
| <a href="/windows/desktop/api/comppkgsup/nf-comppkgsup-aredvdcodecsenabled"><strong>аредвдкодексенаблед</strong></a> | Возвращает значение, указывающее, включены ли на текущем устройстве кодеки DVD.<br /> | 
| <a href="/windows/desktop/api/Winuser/nf-winuser-disableprocesswindowsghosting"><strong>дисаблепроцессвиндовсгхостинг</strong></a> | Отключает функцию дублирования окна для вызывающего графического пользовательского интерфейса. несинхронизированная копия окна — это функция Windows Manager, которая позволяет пользователю легко выполнять, перемещать и закрывать главное окно приложения, которое не отвечает.<br /> | 
| <a href="/windows/desktop/api/comppkgsup/nf-comppkgsup-getmediacomponentpackageinfo"><strong>жетмедиакомпонентпаккажеинфо</strong></a> | Возвращает список свойств для всех кодеков мультимедиа, установленных в системе в соответствии с указанными требованиями.<br /> | 
| <a href="/windows/desktop/api/comppkgsup/nf-comppkgsup-getmediaextensioncommunicationfactory"><strong>жетмедиаекстенсионкоммуникатионфактори</strong></a> | Создает фабрику связи для регистрации расширения мультимедиа.<br /> | 
| <a href="/windows/desktop/api/comppkgsup/nf-comppkgsup-instantiatecomponentfrompackage"><strong>инстантиатекомпонентфромпаккаже</strong></a> | Создает экземпляр класса в пакете приложения. <br /> | 
| <a href="/windows/desktop/api/comppkgsup/nf-comppkgsup-ismediabehaviorenabled"><strong>исмедиабехавиоренаблед</strong></a> | Возвращает значение, указывающее, включен ли режим мультимедиа, связанный с указанным GUID.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-ntclose"><strong>нтклосе</strong></a> | Не рекомендуется. Эта функция используется для закрытия указанного маркера. <a href="/windows/desktop/api/Winternl/nf-winternl-ntclose"><strong>Нтклосе</strong></a> заменяется <a href="/windows/desktop/api/handleapi/nf-handleapi-closehandle">CloseHandle</a>.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-ntdeviceiocontrolfile"><strong>нтдевицеиоконтролфиле</strong></a> | Не рекомендуется. Создает дескрипторы для предоставляемых буферов и передает нетипизированные данные драйверу устройства, связанному с дескриптором файла. <a href="/windows/desktop/api/Winternl/nf-winternl-ntdeviceiocontrolfile"><strong>Нтдевицеиоконтролфиле</strong></a> заменяется <a href="/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol">DeviceIoControl</a>.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-ntwaitforsingleobject"><strong>нтваитфорсинглеобжект</strong></a> | Не рекомендуется. Ожидает, пока указанный объект не выйдет из состояния <code>signaled</code> . <a href="/windows/desktop/api/Winternl/nf-winternl-ntwaitforsingleobject"><strong>Нтваитфорсинглеобжект</strong></a> заменяется объектом <a href="/windows/desktop/api/synchapi/nf-synchapi-waitforsingleobject">WaitForSingleObject</a>.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlansistringtounicodestring"><strong>ртлансистрингтауникодестринг</strong></a> | Преобразует указанную исходную строку ANSI в строку в Юникоде. <br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlchartointeger"><strong>ртлчартоинтежер</strong></a> | Преобразует строку символов в целое число.<br /> | 
| <a href="/previous-versions//ff899322(v=vs.85)"><strong>ртлформаткуррентусеркэйпас</strong></a> | Инициализирует указанный буфер строковым представлением идентификатора безопасности для текущего пользователя. <br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlfreeansistring"><strong>ртлфриансистринг</strong></a> | Освобождает строковый буфер, выделенный <a href="/windows/desktop/api/Winternl/nf-winternl-rtlunicodestringtoansistring"><strong>ртлуникодестрингтоансистринг</strong></a>.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlfreeoemstring"><strong>ртлфриоемстринг</strong></a> | Освобождает строковый буфер, выделенный <a href="/windows/desktop/api/Winternl/nf-winternl-rtlunicodestringtooemstring"><strong>ртлуникодестрингтуемстринг</strong></a>.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlfreeunicodestring"><strong>ртлфриуникодестринг</strong></a> | Освобождает строковый буфер, выделенный <a href="/windows/desktop/api/Winternl/nf-winternl-rtlansistringtounicodestring"><strong>ртлансистрингтауникодестринг</strong></a> или <a href="https://msdn.microsoft.com/library/ms803011.aspx">ртлупкасеуникодестринг</a>.<br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlinitstring"><strong>ртлинитстринг</strong></a> | Инициализирует подсчитанную строку. <br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlinitunicodestring"><strong>ртлинитуникодестринг</strong></a> | Инициализирует подсчитанную строку Юникода. <br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlunicodestringtoansistring"><strong>ртлуникодестрингтоансистринг</strong></a> | Преобразует указанную исходную строку Юникода в строку ANSI. <br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlunicodestringtooemstring"><strong>ртлуникодестрингтуемстринг</strong></a> | Эта функция преобразует указанную исходную строку Юникода в строку OEM. Преобразование выполняется в соответствии с кодовой страницей OEM (OCP). <br /> | 
| <a href="/windows/desktop/api/Winternl/nf-winternl-rtlunicodetomultibytesize"><strong>ртлуникодетомултибитесизе</strong></a> | Определяет, сколько байтов необходимо для представления строки Юникода в виде строки ANSI.<br /> | 
| <a href="/windows/desktop/devnotes/rtlunicodetoutf8n"><strong>RtlUnicodeToUTF8N</strong></a> | Функция <a href="/windows/desktop/devnotes/rtlunicodetoutf8n"><strong>RtlUnicodeToUTF8N</strong></a> преобразует указанную строку Юникода в новую символьную строку, используя 8-разрядную кодовую страницу формата преобразования Юникода (UTF-8).<br /> | 
| <a href="/windows/desktop/devnotes/rtlutf8tounicoden"><strong>RtlUTF8ToUnicodeN</strong></a> | Функция <a href="/windows/desktop/devnotes/rtlutf8tounicoden"><strong>RtlUTF8ToUnicodeN</strong></a> преобразует указанную исходную строку в строку в Юникоде, используя кодовую страницу UTF-8.<br /> | 
| <a href="/windows/desktop/api/Ime/nf-ime-sendimemessageexa"><strong>сендимемессажеекс</strong></a> | Задает действие или обработку для редактора метода ввода (IME) с помощью указанной подфункции.<blockquote>[!Note]<br />Эта функция устарела и не должна использоваться.</blockquote><br /><br /> | 
| <a href="/windows/desktop/api/Winnls32/nf-winnls32-winnlsenableime"><strong>виннлсенаблеиме</strong></a> | Временно включает или отключает редактор IME и в то же время включает или отключает отображение всех окон, принадлежащих редактору IME.<blockquote>[!Note]<br />Эта функция устарела и не должна использоваться.</blockquote><br /><br /> | 




 

### <a name="structures"></a>Структуры



| Раздел                                 | Содержимое                                                                                                                                                                                                                              |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**иместрукт**](/windows/win32/api/ime/ns-ime-imestruct) | Используется функцией [**сендимемессажеекс**](/windows/desktop/api/Ime/nf-ime-sendimemessageexa) для указания подфункции, выполняемой в сообщении IME и его параметрах. Эта структура также используется для получения возвращаемых значений из этих подфункций.<br/> |
| [**STRING**](/windows/desktop/api/Winternl/ns-winternl-string)       | Эта структура используется с функцией [**ртлуникодестрингтуемстринг**](/windows/desktop/api/Winternl/nf-winternl-rtlunicodestringtooemstring) . <br/>                                                                                                              |



 

### <a name="compiler-routines"></a>Подпрограммы компилятора



| Раздел                                                             | Содержимое                                                                                                     |
|-------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| [**\_\_Подпрограммы для \_ конкретного \_ обработчика C**](--c-specific-handler2.md) | [**\_ \_ \_ Специальный \_ обработчик c**](--c-specific-handler2.md) — это вспомогательная подпрограммы для компилятора C.<br/> |
| [\_подпрограммы аллдив](-win32-alldiv.md)                             | [ \_ подпрограммы аллдив](-win32-alldiv.md) — это вспомогательная подпрограммы для компилятора C.<br/>                     |
| [\_аллмул](-win32-allmul.md) | Умножает два **лонглонг** или **улонглонг**. |
| [\_ауллдив](-win32-aulldiv.md) | Делит два целых числа **улонглонг** . |
| [\_подпрограммы чкстк](-win32-chkstk.md)                             | [ \_ подпрограммы чкстк](-win32-chkstk.md) — это вспомогательная подпрограммы для компилятора C.<br/>                     |
