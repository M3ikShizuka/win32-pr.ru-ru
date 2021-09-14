---
description: Комплекты шифров TLS в Windows 8.1
ms.assetid: 48A515C2-96D3-4CBF-A48F-3F0B91F0CB2C
title: Комплекты шифров TLS в Windows 8.1
ms.topic: article
ms.date: 09/10/2021
ms.openlocfilehash: 448473f237a84263239013d833af30ebbfe3ca8e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146522"
---
# <a name="tls-cipher-suites-in-windows-81"></a>Комплекты шифров TLS в Windows 8.1

Комплекты шифров можно согласовать только для тех версий TLS, которые их поддерживают. Наивысшая поддерживаемая версия TLS всегда является предпочтительной в подтверждении TLS. Например, SSL \_ CK \_ RC4 \_ 128 \_ с \_ MD5 можно использовать, только если клиент и сервер не поддерживают TLS 1,2, 1,1 & 1,0 или SSL 3,0, так как он поддерживается только с SSL 2,0.

Доступность комплектов шифров должна контролироваться одним из двух способов:

-   Порядок приоритетов по умолчанию переопределяется при настройке списка приоритетов. Комплекты шифров, отсутствующие в списке приоритетов, не используются.
-   Разрешено, если приложение передает SCH с \_ использованием \_ надежного \_ шифрования: поставщик Microsoft SChannel будет отфильтровывать известные ненадежные наборы шифров, когда приложение использует \_ \_ флаг стойкого \_ шифрования SCH. в Windows 8.1 комплекты шифров RC4 отфильтровываются.

> [!IMPORTANT]
> Веб-службы HTTP/2 завершаются сбоем с комплектами шифров, отличными от HTTP и 2. Сведения о том, как обеспечить работу веб-служб с клиентами и браузерами HTTP/2, см. [в разделе Развертывание настраиваемого упорядочения набора шифров](https://support.microsoft.com/help/4032720/how-to-deploy-custom-cipher-suite-ordering-in-windows-server-2016).

 

Соответствие требованиям FIPS стало более сложным благодаря добавлению эллиптических кривых, что делает столбец с включенным режимом FIPS в предыдущих версиях этой таблицы в заблуждение. Например, набор шифров, например TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256, является жалобой FIPS только при использовании эллиптических кривых NIST. Чтобы узнать, какие сочетания эллиптических кривых и комплектов шифров будут включены в режиме FIPS, ознакомьтесь с разделом 3.3.1 [рекомендаций по выбору, настройке и использованию реализаций TLS]( https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-52r1.pdf).

Windows 8.1 и Windows Server 2012 R2 обновляются Центр обновления Windows с применением [обновления 2919355](https://support.microsoft.com/kb/2919355) , которое добавляет новые комплекты шифров и изменяет порядок приоритета. Следующие комплекты шифров включены и по умолчанию в этом порядке приоритетны поставщиком Microsoft SChannel:



| Строка набора шифров                                                                                            | Разрешено в SCH, \_ использование \_ стойкого \_ шифрования | Версии протокола TLS/SSL                     |
|----------------------------------------------------------------------------------------------------------------|-------------------------------------|-----------------------------------------------|
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA384 \_ P256<br/>                                                  | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA384 \_ P384<br/>                                                  | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256 \_ P256<br/>                                                  | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256 \_ P384<br/>                                                  | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA \_ P256<br/>                                                     | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA \_ P384<br/>                                                     | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA \_ P256<br/>                                                     | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA \_ P384<br/>                                                     | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ дхе \_ RSA \_ с \_ AES \_ 256 \_ gcm \_ SHA384<br/>                                                          | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ дхе \_ RSA \_ с \_ AES \_ 128 \_ gcm \_ SHA256<br/>                                                          | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ дхе \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA<br/>                                                             | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ дхе \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA<br/>                                                             | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ RSA \_ с \_ AES \_ 256 \_ gcm \_ SHA384<br/>                                                               | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ RSA \_ с \_ AES \_ 128 \_ gcm \_ SHA256<br/>                                                               | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA256<br/>                                                               | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256<br/>                                                               | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA<br/>                                                                  | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA<br/>                                                                  | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ gcm \_ SHA384 \_ P384<br/>                                                | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ gcm \_ SHA256 \_ P256<br/>                                                | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ gcm \_ SHA256 \_ P384<br/>                                                | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ CBC \_ SHA384 \_ P384<br/>                                                | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256 \_ P256<br/>                                                | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256 \_ P384<br/>                                                | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ CBC \_ SHA \_ P256<br/>                                                   | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ CBC \_ SHA \_ P384<br/>                                                   | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ CBC \_ SHA \_ P256<br/>                                                   | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ CBC \_ SHA \_ P384<br/>                                                   | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ дхе \_ DSS \_ с \_ AES \_ 256 \_ CBC \_ SHA256<br/>                                                          | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ дхе \_ DSS \_ с \_ AES \_ 128 \_ CBC \_ SHA256<br/>                                                          | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ дхе \_ DSS \_ с \_ AES \_ 256 \_ CBC \_ SHA<br/>                                                             | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ дхе \_ DSS \_ с \_ AES \_ 128 \_ CBC \_ SHA<br/>                                                             | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ RSA \_ с \_ 3DES \_ еде \_ CBC \_ SHA<br/>                                                                 | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ дхе \_ DSS \_ с \_ 3DES \_ еде \_ CBC \_ SHA<br/>                                                            | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| Алгоритм \_ TLS \_ RSA \_ с \_ \_ алгоритмом SHA 128<br/>                                                                       | Нет<br/>                       | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| Алгоритм TLS \_ RSA \_ с \_ RC4 \_ 128 \_ MD5<br/>                                                                       | Нет<br/>                       | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| TLS \_ RSA \_ с \_ нулевым \_ SHA256 <br/> Используется только при явном запросе приложения.<br/>            | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ RSA \_ с \_ нулевым \_ SHA <br/> Используется только при явном запросе приложения.<br/>               | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| SSL \_ CK \_ RC4 \_ 128 \_ с \_ MD5 <br/> Используется только при явном запросе приложения.<br/>            | Нет<br/>                       | SSL 2.0<br/>                            |
| SSL \_ CK \_ Des \_ 192 \_ EDE3 \_ CBC \_ с \_ MD5 <br/> Используется только при явном запросе приложения.<br/> | Да<br/>                      | SSL 2.0<br/>                            |



 

Следующие комплекты шифров поддерживаются поставщиком Schannel (Майкрософт), но не включены по умолчанию.



| Строка набора шифров                                             | Разрешено в SCH, \_ использование \_ стойкого \_ шифрования | Версии протокола TLS/SSL                     |
|-----------------------------------------------------------------|-------------------------------------|-----------------------------------------------|
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA384 \_ P521<br/>   | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256 \_ P521<br/>   | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 256 \_ CBC \_ SHA \_ P521<br/>      | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ RSA \_ с \_ AES \_ 128 \_ CBC \_ SHA \_ P521<br/>      | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ gcm \_ SHA384 \_ P521<br/> | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ gcm \_ SHA256 \_ P521<br/> | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ CBC \_ SHA384 \_ P521<br/> | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ CBC \_ SHA256 \_ P521<br/> | Да<br/>                      | TLS 1.2<br/>                            |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 256 \_ CBC \_ SHA \_ P521<br/>    | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ ECDHE \_ ECDSA \_ с \_ AES \_ 128 \_ CBC \_ SHA \_ P521<br/>    | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0<br/>          |
| TLS \_ RSA \_ с \_ Des \_ CBC \_ SHA<br/>                        | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| TLS \_ RSA \_ EXPORT1024 \_ с \_ \_ \_ алгоритмом SHA 56<br/>             | Нет<br/>                       | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| TLS \_ RSA \_ EXPORT1024 \_ с \_ Des \_ CBC \_ SHA<br/>            | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| \_Экспорт RSA \_ TLS \_ с \_ помощью \_ \_ алгоритма MD5 40<br/>                 | Нет<br/>                       | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| TLS \_ RSA \_ с \_ неопределенным \_ MD5<br/>                            | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| TLS \_ дхе \_ DSS \_ с \_ Des \_ CBC \_ SHA<br/>                   | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| TLS \_ дхе \_ DSS \_ EXPORT1024 \_ с \_ Des \_ CBC \_ SHA<br/>       | Да<br/>                      | TLS 1,2, TLS 1,1, TLS 1,0, SSL 3,0<br/> |
| SSL \_ CK \_ Des \_ 64 \_ CBC \_ с \_ MD5<br/>                     | Да<br/>                      | SSL 2.0<br/>                            |
| SSL \_ CK \_ RC4 \_ 128 \_ EXPORT40 \_ с \_ MD5<br/>               | Нет<br/>                       | SSL 2.0<br/>                            |



 

чтобы добавить комплекты шифров, используйте параметр групповой политики SSL для набора шифров в разделе конфигурация компьютера > административные шаблоны > сеть > конфигурация ssl Параметры, чтобы настроить список приоритетов для всех пакетов шифров, которые требуется включить.

 

 




