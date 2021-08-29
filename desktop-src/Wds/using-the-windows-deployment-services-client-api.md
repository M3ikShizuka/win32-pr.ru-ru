---
title: Использование API клиента служб развертывания Windows
description: в средах, где стандартное решение служб развертывания Windows (WDS) не может использоваться для установки Windows, API клиента WDS позволяет разработчикам создавать пользовательские приложения развертывания.
ms.assetid: abe2a7c7-989a-456e-80df-90d5b816db38
keywords:
- Windows службы развертывания Windows служб развертывания с помощью API клиента
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6840f8327d1576a51d1f3d6cb7b097aaef87abc674bbbba0a004919ef5ce8366
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119760244"
---
# <a name="using-the-windows-deployment-services-client-api"></a>Использование API клиента служб развертывания Windows

в средах, где стандартное решение служб развертывания Windows (WDS) не может использоваться для установки Windows, API клиента WDS позволяет разработчикам создавать пользовательские приложения развертывания. Приложения могут использовать этот API для взаимодействия с сервером WDS для получения сведений о системных образах, доступных на сервере. Пользовательские клиентские приложения WDS должны соответствовать следующим рекомендациям.

## <a name="install-the-wds-role-on-the-server"></a>Установка роли WDS на сервере

-   Windows Службы развертывания (WDS) — это пересмотренная версия служб удаленной установки (RIS), для реализации пользовательских клиентских решений WDS потребуется роль сервера WDS на сервере.
-   WDS заменяет службу RIS стандартным компонентом, начиная с Windows server 2008 и Windows server 2003 с пакетом обновления 2 (SP2).
-   необходимо обновить сервер RIS до WDS на Windows server 2003 с пакетом обновления 1 (SP1). роль сервера WDS можно установить с помощью [пакет автоматической установки Windows (WAIK)](https://www.microsoft.com/download/details.aspx?id=10333).

## <a name="start-windows-pe-20"></a>запуск Windows PE 2,0

Windows PE 2,0 должен быть запущен, если он еще не запущен. клиент WDS и вспомогательные библиотеки dll загружаются только setup.exe, если они находятся на этапе обработки установки Microsoft среда предустановки Windows (Windows PE 2,0).

-   При подключении нового компьютера к сети для загрузки программы сетевой загрузки можно использовать встроенную технологию среды выполнения предзагрузки (PXE). дополнительные сведения о PXE-загрузке компьютера для установки Windows см. в разделе пошаговое описание [обновления служб развертывания Windows](/previous-versions/windows/it-pro/windows-vista/cc766320(v=ws.10)).
-   загрузочный образ RAMDISK Windows PE 2,0 можно сохранить в. Формат WIM и загружается как часть процесса сетевой загрузки. Windows После этого PE можно загрузить и запустить непосредственно с этого носителя.

## <a name="open-a-session-with-the-wds-server"></a>Открытие сеанса с сервером WDS

Клиент WDS должен открыть сеанс с сервером WDS.

-   Используйте функцию [**вдскликреатесессион**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclicreatesession) , чтобы открыть сеанс с сервером WDS. Эта функция принимает имя или IP-адрес сервера и получает адрес маркера для сеанса клиента WDS.
-   Если открытие сеанса с сервером потребует проверки подлинности клиента WDS, то при вызове функции [**вдскликреатесессион**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclicreatesession) приложение должно предоставить адрес структуры [**\_ \_ cred CLI WDS**](/windows/win32/api/wdsclientapi/ns-wdsclientapi-wds_cli_cred) , содержащей учетные данные клиента. Приложение может использовать функцию [**вдсклиаусоризесессион**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscliauthorizesession) для преобразования анонимного сеанса в сеанс, прошедший проверку подлинности.
-   Когда сеанс, Открытый с помощью функции [**вдскликреатесессион**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclicreatesession) , больше не нужен, приложение должно использовать функцию [**вдскликлосе**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscliclose) , чтобы закрыть обработчик и ресурсы освобождения, удерживаемые сеансом.

## <a name="enumerate-system-images-on-the-wds-server"></a>Перечисление образов системы на WDS-сервере

Клиент WDS может использовать API для перечисления образов системы на сервере WDS.

-   Используйте функцию [**вдсклифиндфирстимаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclifindfirstimage) , чтобы получить маркер первого образа и инициализировать перечисление образов на сервере WDS.
-   Используйте функцию [**вдсклифинднекстимаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclifindnextimage) , чтобы увеличить перечисление, запущенное функцией [**вдсклифиндфирстимаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclifindfirstimage) . Функция **вдсклифинднекстимаже** получает маркер для следующего изображения.
-   Используйте функцию [**вдсклижетимажеиндекс**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimageindex) для получения индекса образа для текущего изображения. Это значение допустимо только до тех пор, пока функции [**вдсклифинднекстимаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclifindnextimage) и [**вдскликлосе**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscliclose) не будут использоваться повторно.
-   Используйте функцию [**вдсклижетенумератионфлагс**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetenumerationflags) для получения информационных флагов о фильтрации изображений.

## <a name="get-information-about-images"></a>Получение сведений об образах

Клиент WDS может использовать API для получения сведений об образах на сервере WDS. Следующие функции получают сведения о текущем изображении. Поскольку функции [**вдсклифиндфирстимаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclifindfirstimage) и [**вдсклифинднекстимаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclifindnextimage) изменяют текущее значение обработчика изображения, приложение должно хранить все сведения, которые он получает, и потребуется в будущем перед повторным вызовом функций **вдсклифиндфирстимаже** или **вдсклифинднекстимаже** .

-   Используйте функцию [**вдсклижетимажеарчитектуре**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagearchitecture) для получения архитектуры процессора текущего образа.
-   Используйте функцию [**вдсклижетимажепас**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagepath) , чтобы получить относительный путь к файлу изображения, содержащему текущий образ.
-   Чтобы получить размер изображения, используйте функцию [**вдсклижетимажесизе**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagesize) .
-   Используйте функцию [**вдсклижетимажеверсион**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimageversion) для получения версии образа.
-   Используйте функцию [**вдсклижетимажелангуаже**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagelanguage) , чтобы получить язык по умолчанию для текущего изображения.
-   Используйте функцию [**вдсклижетимажелангуажес**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagelanguages) для получения массива языков, поддерживаемых текущим изображением.
-   Использование [**вдсклижетимажеластмодифиедтиме**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagelastmodifiedtime) Возвращает время последнего изменения для текущего изображения.
-   Чтобы получить имя текущего изображения, используйте функцию [**вдсклижетимаженаме**](/windows/win32/api/WdsClientApi/nf-wdsclientapi-wdscligetimagename) .
-   Используйте функцию [**вдсклижетимажедескриптион**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagedescription) для получения описания текущего изображения.
-   Используйте функцию [**вдсклижетимажеграуп**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagegroup) , чтобы получить имя группы образов для текущего образа.
-   Используйте функцию [**вдсклижетимажехалнаме**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscligetimagehalname) , чтобы получить имя слоя абстрагирования оборудования (HAL) для текущего образа.

## <a name="log-wds-client-events"></a>Регистрация событий клиента WDS

Функция ведения журнала клиентской библиотеки WDS позволяет отправлять события хода установки с клиента на сервер WDS.

-   Используйте функцию [**вдсклиинитиализелог**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdscliinitializelog) для инициализации журнала для сеанса клиента WDS.
-   Используйте функцию [**вдсклилог**](/windows/win32/api/WdsClientAPI/nf-wdsclientapi-wdsclilog) для записи сообщений о событиях в журнал сервера WDS.
-   на Windows server 2008 сервер WDS записывает события клиента в журнал событий конкретного приложения, который можно просмотреть с помощью eventvwr.exe, а также журнала трассировки отладки. на Windows server 2003 с включенным ведением журнала отладки сервер WDS будет записывать события клиента в файл журнала, расположенный в папке% windir% \\ tracing \\ wdsserver. log. Для захвата этих событий необходимо включить ведение журнала клиента WDS на сервере.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[сведения об API служб развертывания Windows](about-the-windows-deployment-services-api.md)
</dt> <dt>

[Использование API сервера служб развертывания Windows](using-the-windows-deployment-services-server-api.md)
</dt> </dl>

 

 