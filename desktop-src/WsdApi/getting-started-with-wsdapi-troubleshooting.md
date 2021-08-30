---
description: Существует два способа определения используемой процедуры диагностики.
ms.assetid: d6877063-6cf9-48dc-8208-0f3fc85b6d6b
title: начало работы с разрешениями WSDAPI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7dec7fc848fddf412bde43a4f2cb94021b382820
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122474910"
---
# <a name="getting-started-with-wsdapi-troubleshooting"></a>начало работы с разрешениями WSDAPI

Это руководство по устранению неполадок содержит набор [диагностических процедур](wsdapi-diagnostic-procedures.md) , которые можно использовать для выявления причины проблем с приложениями. После успешного определения причины проблемы можно применить предлагаемые решения в процедуре диагностики, чтобы устранить проблему.

Существует два способа определения используемой процедуры диагностики. Один из способов — перейти на страницу устранения неполадок для типа клиента, чтобы просмотреть пошаговый список процедур диагностики, используемых для устранения неполадок клиента. Другой способ — перейти на краткий справочник по устранению неполадок, чтобы просмотреть сводные таблицы, демонстрирующие распространенные проблемы с приложениями WSDAPI и процедуры, используемые для диагностики проблем.

## <a name="troubleshooting-by-type-of-client"></a>Устранение неполадок по типу клиента

В следующих разделах представлены соответствующие диагностические процедуры по типу клиента. В этих разделах также показаны шаблоны сообщений, связанные с типом клиента.

-   [Устранение неполадок приложений WSDAPI с использованием направленного обнаружения](troubleshooting-applications-using-directed-discovery.md)
-   [Устранение неполадок клиентов обнаружения функций](troubleshooting-function-discovery-clients.md)
-   [Устранение неполадок соседних пользователей и собраний](troubleshooting-people-near-me-meetings-near-me.md)
-   [Устранение неполадок мастера добавления принтера](troubleshooting-the-add-printer-wizard.md)
-   [Устранение неполадок обозревателя сети](troubleshooting-the-network-explorer.md)
-   [Устранение неполадок мастера проекторов](troubleshooting-the-projector-wizard.md)
-   [Устранение неполадок других приложений WSDAPI](troubleshooting-wsdapi-applications.md)

## <a name="troubleshooting-quick-reference"></a>Краткий справочник по устранению неполадок

В следующих таблицах показаны некоторые проблемы, которые могут препятствовать тому, что клиенты и узлы WSDAPI видят друг друга в сети и не обмениваются метаданными устройства. В таблицах также показаны выполняемые процедуры диагностики и критерии, используемые для определения того, страдает ли приложение от определенной проблемы.

### <a name="network-environment-problems"></a>Проблемы с сетевой средой



| Проблема                                                                                                                                                                                              | Диагностическая процедура                                                                                                                                                                                                                             | Идентификация проблемы                                                                                                                                                                            |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Брандмауэр блокирует трафик сетевого обнаружения.                                                                                                                                                       | [проверка Параметры адаптера и брандмауэра](inspecting-adapter-and-firewall-settings.md)                                                                                                                                                         | Включение исключения обнаружения сетевых ошибок в брандмауэре решает эту проблему.                                                                                                                      |
| Исключения брандмауэра, характерные для приложения, блокируют сообщения.                                                                                                                               | [проверка Параметры адаптера и брандмауэра](inspecting-adapter-and-firewall-settings.md)                                                                                                                                                         | Отключение брандмауэра решает проблему. WF. msc показывает правила брандмауэра, зависящие от приложения.                                                                                                      |
| Устройство не отвечает на UDP-запросы, отправляя сообщение [ProbeMatch](probematches-message.md) или [ресолвематчес](resolvematches-message.md) своевременно (менее 4 секунд). | [проверка Параметры адаптера и брандмауэра](inspecting-adapter-and-firewall-settings.md)                                                                                                                                                         | Отключение брандмауэра решает проблему, и универсальный узел, который реагирует менее 4 секунд, работает успешно.                                                                            |
| Неправильный контекст безопасности приложения (т. е. Клиент и узел не имеют достаточных разрешений в сети).                                                                 | [Использование универсального узла и клиента для протокола UDP WS-Discovery](using-a-generic-host-and-client-for-udp-ws-discovery.md) или [универсального узла и клиента для метаданных HTTP Exchange](using-a-generic-host-and-client-for-http-metadata-exchange.md) | Адрес устройства не отображается в выходных данных клиента отладки WSD. Запуск приложения от имени администратора решает проблему.                                                                          |
| Политика IPSec блокирует сообщения.                                                                                                                                                                | [Использование универсального узла и клиента для протокола UDP WS-Discovery](using-a-generic-host-and-client-for-udp-ws-discovery.md) или [универсального узла и клиента для метаданных HTTP Exchange](using-a-generic-host-and-client-for-http-metadata-exchange.md) | Адрес устройства не отображается в выходных данных клиента отладки WSD. Проблема не устранена путем отключения брандмауэра. Эта проблема не может быть воспроизведена на компьютере, не подчиняются политикам IPSec. |



 

### <a name="discovery-traffic-problems"></a>Проблемы с трафиком обнаружения




| Проблема | Диагностическая процедура | Идентификация проблемы | 
|---------|----------------------|------------------------|
| Сообщения <a href="hello-message.md">Hello</a>, <a href="probe-message.md">зонд</a>или <a href="resolve-message.md">Resolve</a> не передаются в сети, так как приложение неправильно перечисляет сетевые интерфейсы многоадресной рассылки. | <a href="using-wsddebug-client-to-verify-multicast-traffic.md">Использование клиента отладки WSD для проверки трафика многоадресной рассылки</a> | Сообщения Hello, зонд или Resolve не отображаются в выходных данных клиента отладки WSD. Пакеты не отображаются в сети. Пакеты не формируются для интерфейса замыкания на себя или для других интерфейсов. | 
| Сообщения <a href="probe-message.md">пробы</a> не отправляются с помощью многоадресной рассылки UDP на порт 3702 (для приложений, не использующих управляемое обнаружение). | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> | Проверка сообщения показывает, что оно было отправлено на неправильный порт. | 
| Сообщение <a href="probe-message.md">пробы</a> не содержит элемент <strong>types</strong> , или элемент <strong>types</strong> пуст. | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка сообщения показывает, что элемент <strong>types</strong> отсутствует или пуст. | 
| Элемент <strong>types</strong> сообщения <a href="probe-message.md">пробы</a> не содержит типы, на которые будет отвечать узел. | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка сообщения показывает, что элемент <strong>types</strong> содержит неправильно сформированное или неверное значение. | 
| Сообщение <a href="probematches-message.md">ProbeMatch</a> не было отправлено по АДРЕСу UDP-порту, с которого была отправлена <a href="probe-message.md">проба</a> . | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка выходных данных показывает, что сообщение <a href="probematches-message.md">ProbeMatch</a>) не было отправлено, или сообщение было отправлено на неправильный порт.<blockquote>[!Note]<br />Для приложений, использующих управляемое обнаружение, <a href="probematches-message.md">ProbeMatch</a> должен быть отправлен по протоколу HTTP или HTTPS в ответ на сообщение <a href="probe-message.md">пробы</a> .</blockquote><br /> | 
| Сообщение <a href="probematches-message.md">ProbeMatch</a> не содержит элемент очистки, <strong>или элемент «</strong> текст сообщения <strong>» пуст</strong> . | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка сообщения показывает, <strong>что элемент очистки</strong> отсутствует или пуст. | 
| Значение <strong>элемента «текст</strong> сообщения об ошибке» в сообщении <a href="probematches-message.md">ProbeMatch</a> не соответствует значению элемента <strong>MessageId</strong> из соответствующего сообщения <a href="probe-message.md">зонда</a> . | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка сообщения показывает, что <strong>элемент «текст</strong> сообщения» содержит неправильно сформированное или неверное значение. | 
| Элемент <strong>ксаддрс</strong> , входящий в сообщение <a href="probematches-message.md">ProbeMatch</a> , не соответствует <a href="xaddr-validation-rules.md">правилам проверки ксаддр</a>. | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка сообщения показывает, что <strong>ксаддрс</strong> являются недопустимыми. | 
| <a href="resolve-message.md">Разрешение</a> сообщений не отправляется с помощью многоадресной рассылки UDP на порт 3702 (для приложений, не использующих направленное обнаружение). | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка выходных данных показывает, что сообщение <a href="resolve-message.md">разрешения</a> было отправлено на неправильный порт. | 
| Сообщение <a href="resolvematches-message.md">ресолвематчес</a> не было отправлено по адресу UDP-порту, с которого было отправлено сообщение <a href="resolve-message.md">разрешения</a> . | <a href="inspecting-network-traces-for-udp-ws-discovery.md">Проверка трассировки сети для протокола UDP WS-Discovery</a> или <a href="inspecting-network-traces-for-applications-using-directed-discovery.md">изучение трассировок сети для приложений, использующих</a> управляемое обнаружение | Проверка выходных данных показывает, что сообщение <a href="resolvematches-message.md">ресолвематчес</a> не было отправлено или сообщение было отправлено на неправильный порт. | 




 

### <a name="metadata-exchange-problems"></a>Проблемы обмена метаданными




| Проблема | Диагностическая процедура | Идентификация проблемы | 
|---------|----------------------|------------------------|
| Адрес транспорта, объявленный узлом, неверен. | <a href="using-a-generic-host-and-client-for-http-metadata-exchange.md">Использование универсального узла и клиента для метаданных HTTP Exchange</a> | Проверка Ксаддрс в выходных данных клиента отладки WSD показывает, что транспортный адрес неправильный или имеет неправильный формат. | 
| Не удалось установить TCP-соединение для обмена метаданными. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | Выходные данные анализатора пакетов не показывают следующий обмен пакетами:<ul><li>Пакет SYN TCP, отправленный клиентом</li><li>Пакет TCP SYN/ACK, отправленный с узла</li><li>Пакет TCP ACK, отправленный клиентом</li></ul> | 
| Клиент не отправил допустимый HTTP-запрос GET. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | В выходных данных анализатора пакетов нет HTTP-запроса GET, или запрос имеет неправильный формат. | 
| Клиент не отправлял допустимое сообщение WS-Transfer <a href="get--metadata-exchange--http-request-and-message.md">получения</a> . | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | В выходных данных анализатора пакетов отсутствует WS-Transfer сообщение <a href="get--metadata-exchange--http-request-and-message.md">Get</a> , или сообщение имеет неправильный формат. | 
| Узел не прослушивает URL-путь, указанный в HTTP-запросе GET. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | В выходных данных анализатора пакетов нет HTTP-ответа. | 
| Сообщение WS-Transfer <a href="get--metadata-exchange--http-request-and-message.md">Get</a> не содержит элемент <strong>to</strong> , либо элемент <strong>to</strong> пуст. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | Проверка сообщения показывает, что элемент <strong>to</strong> отсутствует или пуст. | 
| Значение элемента <strong>To</strong> WS-Transferного сообщения <a href="get--metadata-exchange--http-request-and-message.md">Get</a> не соответствует одному из адресов конечной точки узла. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | Проверка сообщения показывает, что значение элемента <strong>to</strong> не соответствует одному из адресов конечной точки, объявленных в сообщении <a href="probematches-message.md">ProbeMatch</a> или <a href="resolvematches-message.md">ресолвематчес</a> узла. | 
| Узел не отправил допустимый заголовок HTTP-ответа. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | В выходных данных анализатора пакетов отсутствует HTTP-ответ, или запрос имеет неправильный формат. | 
| Заголовок ответа HTTP, отправленный узлом, указывает на то, что запрос не может быть выполнен. | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | Заголовок ответа имеет код состояния, отличный от HTTP/1.1 200. | 
| Узел не отправил допустимое сообщение <a href="getresponse--metadata-exchange--message.md">GetResponse</a> . | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | В выходных данных анализатора пакетов отсутствует сообщение <a href="getresponse--metadata-exchange--message.md">GetResponse</a> , или сообщение имеет неправильный формат. | 
| Сообщение <a href="getresponse--metadata-exchange--message.md">GetResponse</a> не <strong>содержит элемента очистки</strong> , или <strong>элемент «текст сообщения» пуст</strong> . | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | Проверка сообщения показывает, <strong>что элемент очистки</strong> отсутствует или пуст. | 
| Значение <strong>элемента «текст</strong> сообщения об ошибке» в сообщении <a href="getresponse--metadata-exchange--message.md">GetResponse</a> не соответствует значению элемента <strong>MessageId</strong> из соответствующего сообщения <a href="get--metadata-exchange--http-request-and-message.md">Get</a> . | <a href="inspecting-network-traces-for-http-metadata-exchange.md">Проверка трассировки сети для Exchange метаданных HTTP</a> | Проверка сообщения показывает, что <strong>элемент «текст</strong> сообщения» содержит неправильно сформированное или неверное значение. | 


## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Руководство по устранению неполадок WSDAPI](wsdapi-troubleshooting-guide.md)
</dt> </dl>
