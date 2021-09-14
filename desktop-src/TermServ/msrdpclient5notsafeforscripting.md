---
title: Класс MsRdpClient5NotSafeForScripting
description: Клиентский элемент управления Microsoft RDP — версия 6.
ms.assetid: 0DC46910-D77E-47CF-92C3-4019D79C783C
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов класса MsRdpClient5NotSafeForScripting
- Службы удаленных рабочих столов класс MsRdpClient5NotSafeForScripting, описание
topic_type:
- apiref
api_name:
- MsRdpClient5NotSafeForScripting
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6b3fd7c6a34024e15907bd4e41b93ce693b18ce8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968053"
---
# <a name="msrdpclient5notsafeforscripting-class"></a>Класс MsRdpClient5NotSafeForScripting

Клиентский элемент управления Microsoft RDP — версия 6

Этот класс реализует следующие интерфейсы.

-   [**IMsRdpClient5**](imsrdpclient5.md)
-   [**IMsRdpClient4**](imsrdpclient4.md)
-   [**IMsRdpClient3**](imsrdpclient3.md)
-   [**IMsRdpClient2**](imsrdpclient2.md)
-   [**имсрдпклиент**](imsrdpclientshell2.md)
-   [**имстскакс**](imstscax-interface.md)
-   [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch)
-   [**имстскаксевентс**](imstscaxevents-interface.md)
-   [**имстскнонскриптабле**](imstscnonscriptable-interface.md)
-   [**имсрдпклиентнонскриптабле**](imsrdpclientnonscriptable-interface.md)
-   [**IMsRdpClientNonScriptable2**](imsrdpclientnonscriptable2.md)
-   [**IMsRdpClientNonScriptable3**](imsrdpclientnonscriptable3.md)

**MsRdpClient5NotSafeForScripting** имеет следующие типы членов:

-   [Методы](#methods)
-   [Свойства](#properties)

### <a name="methods"></a>Методы

Класс **MsRdpClient5NotSafeForScripting** содержит следующие методы.



| Метод                                                                                      | Описание                                                                                                                                                                                                                                                                                   |
|:--------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Подключение**](imstscax-connect.md)                                                         | Инициирует соединение с использованием свойств, заданных в данный момент в элементе управления.<br/>                                                                                                                                                                                                          |
| [**креатевиртуалчаннелс**](imstscax-createvirtualchannels.md)                             | Создает объект виртуального канала на стороне клиента для каждого указанного имени виртуального канала.<br/>                                                                                                                                                                                              |
| [**Отключение**](imstscax-disconnect.md)                                                   | Отключает активное подключение.<br/>                                                                                                                                                                                                                                                 |
| [**жетеррордескриптион**](imsrdpclient5-geterrordescription.md)                            | Получает коды ошибок и сообщения об ошибках.<br/>                                                                                                                                                                                                                                      |
| [**жетвиртуалчаннелоптионс**](imsrdpclient-getvirtualchanneloptions.md)                   | Извлекает параметры, заданные для виртуального канала.<br/>                                                                                                                                                                                                                                   |
| [**нотифиредиректдевицечанже**](imsrdpclientnonscriptable-notifyredirectdevicechange.md)  | сообщает модулю перенаправления устройств элемента управления удаленный рабочий стол ActiveX, что в системе произошло изменение устройства. Этот метод передает в элемент управления уведомления [**WM \_ девицечанже**](/windows/desktop/DevIO/wm-devicechange) .<br/>                                                        |
| [**онаусентикатионварнингдисмиссед**](imstscaxevents-onauthenticationwarningdismissed.md) | вызывается после того, как элемент управления "ActiveX" отображает диалоговое окно проверки подлинности (например, диалоговое окно "ошибка сертификата").<br/>                                                                                                                                                             |
| [**онаусентикатионварнингдисплайед**](imstscaxevents-onauthenticationwarningdisplayed.md) | вызывается перед тем, как элемент управления ActiveX отображает диалоговое окно проверки подлинности (например, диалоговое окно "ошибка сертификата").<br/>                                                                                                                                                            |
| [**онаутореконнектед**](imstscaxevents-onautoreconnected.md)                               | Вызывается при автоматическом повторном подключении клиентского элемента управления к удаленному сеансу.<br/>                                                                                                                                                                                                  |
| [**онаутореконнектинг**](-imstscaxevents--onautoreconnecting.md)                           | Вызывается, когда клиент находится в процессе автоматического повторного подключения к сеансу с сервером узла сеансов удаленных рабочих столов.<br/>                                                                                                                                                                      |
| [**OnAutoReconnecting2**](imstscaxevents-onautoreconnecting2.md)                           | Вызывается, когда клиент находится в процессе автоматического повторного подключения к сеансу с сервером узла сеансов удаленных рабочих столов.<br/>                                                                                                                                                                      |
| [**ончаннелрецеиведдата**](imstscaxevents-onchannelreceiveddata.md)                       | Вызывается, когда клиент получает данные в виртуальном канале, поддерживающем скрипт.<br/>                                                                                                                                                                                                              |
| [**онконфирмклосе**](imstscaxevents-onconfirmclose.md)                                     | Вызывается, когда клиент вызывает метод [**имсрдпклиент:: RequestClose**](imsrdpclient-requestclose.md) .<br/>                                                                                                                                                                           |
| [**Подключено**](imstscaxevents-onconnected.md)                                           | Вызывается, когда клиентский элемент управления находится в процессе установления соединения с сервером узла сеансов удаленных рабочих столов.<br/>                                                                                                                                                                       |
| [**Подключение**](imstscaxevents-onconnecting.md)                                         | вызывается, когда клиентский элемент управления начинает подключаться к серверу в ответ на вызов [**имстскакс:: Подключение**](imstscax-connect.md).<br/>                                                                                                                                               |
| [**онконнектионбарпуллдовн**](imstscaxevents-onconnectionbarpulldown.md)                   | Вызывается, когда пользователь перетаскивается на панель подключения.<br/>                                                                                                                                                                                                                       |
| [**ондевицесбуттонпрессед**](imstscaxevents-ondevicesbuttonpressed.md)                     | Вызывается при нажатии кнопки устройства на панели подключения.<br/>                                                                                                                                                                                                             |
| [**С отключением**](imstscaxevents-ondisconnected.md)                                     | Вызывается, когда клиентский элемент управления был отключен от сервера узла сеансов удаленных рабочих столов.<br/>                                                                                                                                                                                              |
| [**онентерфуллскринмоде**](imstscaxevents-onenterfullscreenmode.md)                       | Вызывается, когда клиент переходит в полноэкранный режим. Например, это событие вызывается при нажатии [пользователем сочетания клавиш](terminal-services-shortcut-keys.md) в полноэкранном режиме (Ctrl + Alt + Break).<br/>                                                                     |
| [**онфаталеррор**](imstscaxevents-onfatalerror.md)                                         | Вызывается, когда клиентский элемент управления обнаруживает неустранимую ошибку.<br/>                                                                                                                                                                                                                           |
| [**онфокусрелеасед**](imstscaxevents-onfocusreleased.md)                                   | Вызывается при нажатии сочетания клавиш для фокуса в выпуске. Например, это событие вызывается, когда пользователь нажимает клавишу CTRL + ALT + стрелка влево или сочетание клавиш CTRL + ALT + стрелка вправо.<br/>                                                                                             |
| [**онидлетимеаутнотификатион**](imstscaxevents-onidletimeoutnotification.md)               | Вызывается, когда пользователь не наводит мышь или клавиатуру в течение периода времени, заданного методом [**имсрдпклиентадванцедсеттингс::p UT \_ минутестоидлетимеаут**](imsrdpclientadvancedsettings-minutestoidletimeout.md) .<br/>                                                |
| [**онлеавефуллскринмоде**](imstscaxevents-onleavefullscreenmode.md)                       | Вызывается, когда клиент выходит из полноэкранного режима. Например, это событие вызывается при нажатии [пользователем сочетания клавиш](terminal-services-shortcut-keys.md) в полноэкранном режиме (Ctrl + Alt + Break).<br/>                                                                     |
| [**онлогинкомплете**](imstscaxevents-onlogincomplete.md)                                   | вызывается, когда клиентский элемент управления успешно выполнил вход на сервер узла сеансов удаленных рабочих столов, как показано в диалоговом окне входа Windows.<br/>                                                                                                                                      |
| [**онлогонеррор**](imstscaxevents-onlogonerror.md)                                         | Вызывается при возникновении ошибки входа в систему или другого события входа.<br/>                                                                                                                                                                                                                             |
| [**онмаусеинпутмодечанжед**](imstscaxevents-onmouseinputmodechanged.md)                   | Вызывается при изменении режима ввода с помощью мыши.<br/>                                                                                                                                                                                                                                      |
| [**оннетворкстатусчанжед**](imstscaxevents-onnetworkstatuschanged.md)                     | Вызывается при изменении состояния сети.<br/>                                                                                                                                                                                                                                        |
| [**онрецеиведтспубликкэй**](imstscaxevents-onreceivedtspublickey.md)                       | Вызывается во время последовательности подключения, когда клиент получает открытый ключ с сервера. Это событие вызывается, только если свойство **нотифитспубликкэй** имеет значение **Variant \_ true**.<br/>                                                                                              |
| [**онремотедесктопсизечанже**](imstscaxevents-onremotedesktopsizechange.md)               | Вызывается для указания того, что размер клиентского элемента управления в удаленном рабочем столе изменился в ответ на операцию клиентского управления.<br/>                                                                                                                                                |
| [**онремотепрограмдисплайед**](imstscaxevents-onremoteprogramdisplayed.md)                 | Вызывается при отображении программы RemoteApp.<br/>                                                                                                                                                                                                                                      |
| [**онремотепрограмресулт**](imstscaxevents-onremoteprogramresult.md)                       | Вызывается, когда программа RemoteApp возвращает результат в клиентский элемент управления.<br/>                                                                                                                                                                                                            |
| [**онремотевиндовдисплайед**](imstscaxevents-onremotewindowdisplayed.md)                   | Вызывается при отображении окна RemoteApp.<br/>                                                                                                                                                                                                                                       |
| [**онрекуестконтаинерминимизе**](imstscaxevents-onrequestcontainerminimize.md)             | Вызывается, когда пользователь нажимает кнопку **сворачивания** на панели подключения в полноэкранном режиме. Срабатывание этого события является запрос, в котором приложение контейнера свернется само по себе.<br/>                                                                                              |
| [**онрекуестгофуллскрин**](imstscaxevents-onrequestgofullscreen.md)                       | Вызывается, когда клиент запрашивает переключение в полноэкранный режим и вызывается метод [**имстскадванцедсеттингс::p UT \_ контаинерхандледфуллскрин**](imstscadvancedsettings-containerhandledfullscreen.md) , чтобы установить свойство **контаинерхандледфуллскрин** в ненулевое значение.<br/> |
| [**онрекуестлеавефуллскрин**](imstscaxevents-onrequestleavefullscreen.md)                 | Вызывается, когда клиент запрашивает, чтобы выйти из полноэкранного режима, а свойство [**имстскадванцедсеттингс::p UT \_ контаинерхандледфуллскрин**](imstscadvancedsettings-containerhandledfullscreen.md) установлено в ненулевое значение.<br/>                                                   |
| [**онсервицемессажерецеивед**](imstscaxevents-onservicemessagereceived.md)                 | Вызывается, когда клиент получает системное сообщение.<br/>                                                                                                                                                                                                                                  |
| [**онусернамеаккуиред**](imstscaxevents-onusernameacquired.md)                             | Вызывается, когда имя пользователя было получено элементом управления.<br/>                                                                                                                                                                                                                        |
| [**OnWarning**](imstscaxevents-onwarning.md)                                               | Вызывается, когда клиентский элемент управления обнаруживает неустранимое условие ошибки.<br/>                                                                                                                                                                                                    |
| [**RequestClose**](imsrdpclient-requestclose.md)                                           | Запрашивает корректное завершение работы клиентского элемента управления.<br/>                                                                                                                                                                                                                                |
| [**ресетпассворд**](imstscnonscriptable-resetpassword.md)                                  | Сбрасывает все состояния паролей в элементе управления.<br/>                                                                                                                                                                                                                                         |
| [**SendKeys**](imsrdpclientnonscriptable-sendkeys.md)                                      | Отправляет в элемент управления ряд нажатий клавиш. Нажатия клавиш находятся в форме кода сканирования, которая является данными клавиатуры из фактических физических ключей.<br/>                                                                                                                                       |
| [**сендонвиртуалчаннел**](imstscax-sendonvirtualchannel.md)                               | Отправляет данные на сервер узла сеансов удаленных рабочих столов по виртуальному каналу, созданному ранее с помощью метода [**имстскакс:: креатевиртуалчаннелс**](imstscax-createvirtualchannels.md) .<br/>                                                                                         |
| [**сетвиртуалчаннелоптионс**](imsrdpclient-setvirtualchanneloptions.md)                   | Задает параметры виртуального канала для клиентского элемента управления.<br/>                                                                                                                                                                                                                           |



 

### <a name="properties"></a>Свойства

Класс **MsRdpClient5NotSafeForScripting** имеет следующие свойства.




| Свойство | Тип доступа | Описание | 
|----------|-------------|-------------|
| <a href="imstscax-advancedsettings.md"><strong>адванцедсеттингс</strong></a><br /> | Только для чтения<br /> | Указатель интерфейса <a href="imstscadvancedsettings-interface.md"><strong>имстскадванцедсеттингс</strong></a> .<br /> | 
| <a href="imsrdpclient-advancedsettings2.md"><strong>AdvancedSettings2</strong></a><br /> | Только для чтения<br /> | Указатель на интерфейс <a href="imsrdpclientadvancedsettings-interface.md"><strong>имсрдпклиентадванцедсеттингс</strong></a> , используемый для задания дополнительных параметров клиентского элемента управления.<br /> | 
| <a href="imsrdpclient2-advancedsettings3.md"><strong>AdvancedSettings3</strong></a><br /> | Только для чтения<br /> | Указатель на интерфейс <a href="imsrdpclientadvancedsettings2.md"><strong>IMsRdpClientAdvancedSettings2</strong></a> , используемый для задания дополнительных параметров клиентского элемента управления.<br /> | 
| <a href="imsrdpclient3-advancedsettings4.md"><strong>AdvancedSettings4</strong></a><br /> | Только для чтения<br /> | Указатель на интерфейс <a href="imsrdpclientadvancedsettings3.md"><strong>IMsRdpClientAdvancedSettings3</strong></a> , используемый для задания дополнительных параметров клиентского элемента управления.<br /> | 
| <a href="imsrdpclient4-advancedsettings5.md"><strong>AdvancedSettings5</strong></a><br /> | Только для чтения<br /> | Указатель интерфейса <a href="imsrdpclientadvancedsettings4.md"><strong>IMsRdpClientAdvancedSettings4</strong></a> .<br /> | 
| <a href="imsrdpclient5-advancedsettings6.md"><strong>AdvancedSettings6</strong></a><br /> | Только для чтения<br /> | Интерфейс для <a href="imsrdpclientadvancedsettings5.md"><strong>IMsRdpClientAdvancedSettings5</strong></a>.<br /> | 
| <a href="imstscnonscriptable-binarypassword.md"><strong>бинарипассворд</strong></a><br /> | Чтение/запись<br /> | Данное свойство не поддерживается.<br /> | 
| <a href="imstscnonscriptable-binarysalt.md"><strong>бинарисалт</strong></a><br /> | Чтение/запись<br /> | Данное свойство не поддерживается.<br /> | 
| <a href="imstscax-cipherstrength.md"><strong>Циферстренгс</strong></a><br /> | Только для чтения<br /> | Максимальная стойкость шифрования текущего элемента управления.<br /> | 
| <a href="imstscnonscriptable-cleartextpassword.md"><strong>клеартекстпассворд</strong></a><br /> | Только на запись<br /> | пароль удаленный рабочий стол ActiveX управления в текстовом формате.<br /> | 
| <a href="imsrdpclient-colordepth.md"><strong>Clientareawidth</strong></a><br /> | Чтение/запись<br /> | Глубина цвета текущего элемента управления.<br /> | 
| <a href="imstscax-connected.md"><strong>Организован</strong></a><br /> | Только для чтения<br /> | Состояние соединения текущего элемента управления.<br /> | 
| <a href="imsrdpclient2-connectedstatustext.md"><strong>коннектедстатустекст</strong></a><br /> | Чтение/запись<br /> | Текст, отображаемый в клиентской области элемента управления, когда элемент управления находится в состоянии Connected.<br /> | 
| <a href="imstscax-connectingtext.md"><strong>коннектингтекст</strong></a><br /> | Чтение/запись<br /> | Текст, отображаемый по центру элемента управления во время подключения элемента управления.<br /> | 
| <a href="imsrdpclientnonscriptable3-connectionbartext.md"><strong>коннектионбартекст</strong></a><br /> | Чтение/запись<br /> | Текстовая строка, отображаемая для панели подключения.<br /> | 
| <a href="imstscax-desktopheight.md"><strong>десктофеигхт</strong></a><br /> | Чтение/запись<br /> | Высота текущего элемента управления (в пикселях) на начальном удаленном рабочем столе.<br /> | 
| <a href="imstscax-desktopwidth.md"><strong>десктопвидс</strong></a><br /> | Чтение/запись<br /> | Ширина текущего элемента управления (в пикселях) на начальном удаленном рабочем столе.<br /> | 
| <a href="imsrdpclientnonscriptable3-devicecollection.md"><strong>Описания</strong></a><br /> | Только для чтения<br /> | Коллекция устройств PnP, доступных для перенаправления.<br /> | 
| <a href="imstscax-disconnectedtext.md"><strong>дисконнектедтекст</strong></a><br /> | Чтение/запись<br /> | Текст, отображаемый по центру элемента управления до завершения соединения.<br /> | 
| <a href="imstscax-domain.md"><strong>Домен</strong></a><br /> | Чтение/запись<br /> | Домен, в который входит текущий пользователь.<br /> | 
| <a href="imsrdpclientnonscriptable3-drivecollection.md"><strong>дривеколлектион</strong></a><br /> | Только для чтения<br /> | Коллекция дисков, доступная для перенаправления.<br /> | 
| <a href="imsrdpclientnonscriptable3-enablecredsspsupport.md"><strong>енаблекредсспсуппорт</strong></a><br /> | Чтение/запись<br /> | Указывает, включен ли CredSSP для этого соединения.<br /> | 
| <a href="imsrdpclient-extendeddisconnectreason.md"><strong>екстендеддисконнектреасон</strong></a><br /> | Только для чтения<br /> | Расширенные сведения о причине отключения клиентского элемента управления.<br /> | 
| <a href="imsrdpclient-fullscreen.md"><strong>FullScreen</strong></a><br /> | Чтение/запись<br /> | Указывает, находится ли элемент управления в полноэкранном режиме.<br /> | 
| <a href="imstscax-fullscreentitle.md"><strong>фуллскринтитле</strong></a><br /> | Только на запись<br /> | Заголовок окна, отображаемый, если элемент управления находится в полноэкранном режиме.<br /> | 
| <a href="imstscax-horizontalscrollbarvisible.md"><strong>хоризонталскроллбарвисибле</strong></a><br /> | Только для чтения<br /> | Указывает, отображает ли элемент управления горизонтальную полосу прокрутки.<br /> | 
| <a href="imsrdpclient5-msrdpclientshell.md"><strong>мсрдпклиентшелл</strong></a><br /> | Только для чтения<br /> | Параметры клиента для средства запуска веб-портала.<br /> | 
| <a href="imsrdpclientnonscriptable3-negotiatesecuritylayer.md"><strong>неготиатесекуритилайер</strong></a><br /> | Чтение/запись<br /> | Указывает, поддерживается ли параметр Неготиатесекуритилайер для этого соединения.<br /><blockquote>[!Note]<br />Если <a href="imsrdpclientnonscriptable3-enablecredsspsupport.md"><strong>кредсспсуппорт</strong></a> включен и находится на клиенте или если SSL (SSL) включен с проверкой подлинности пользователя, неготиатесекуритилайер игнорируется.</blockquote><br /> | 
| <a href="imstscnonscriptable-portablepassword.md"><strong>портаблепассворд</strong></a><br /> | Чтение/запись<br /> | Данное свойство не поддерживается.<br /> | 
| <a href="imstscnonscriptable-portablesalt.md"><strong>портаблесалт</strong></a><br /> | Чтение/запись<br /> | Данное свойство не поддерживается.<br /> | 
| <a href="imsrdpclientnonscriptable3-promptforcredentials.md"><strong>промптфоркредентиалс</strong></a><br /> | Чтение/запись<br /> | Указывает, следует ли отображать диалоговое окно Запрос учетных данных.<br /> | 
| <a href="imsrdpclientnonscriptable3-redirectdynamicdevices.md"><strong>редиректдинамикдевицес</strong></a><br /> | Чтение/запись<br /> | Указывает, доступны ли для перенаправления динамически подключаемые устройства PnP, перечисленные в сеансе.<br /> | 
| <a href="imsrdpclientnonscriptable3-redirectdynamicdrives.md"><strong>редиректдинамикдривес</strong></a><br /> | Чтение/запись<br /> | Указывает, доступны ли для перенаправления динамически подключаемые диски PnP, перечисленные в сеансе.<br /> | 
| <a href="imsrdpclient5-remoteprogram.md"><strong>ремотепрограм</strong></a><br /> | Только для чтения<br /> | Параметр клиента RemoteApp.<br /> | 
| <a href="imstscax-securedsettings.md"><strong>секуредсеттингс</strong></a><br /> | Только для чтения<br /> | Указатель интерфейса <a href="imstscsecuredsettings-interface.md"><strong>имстсксекуредсеттингс</strong></a> .<br /> | 
| <a href="imsrdpclient-securedsettings2.md"><strong>SecuredSettings2</strong></a><br /> | Только для чтения<br /> | Указатель на интерфейс <a href="imsrdpclientsecuredsettings-interface.md"><strong>имсрдпклиентсекуредсеттингс</strong></a> , используемый для задания защищенных параметров клиентского элемента управления.<br /> | 
| <a href="imstscax-securedsettingsenabled.md"><strong>секуредсеттингсенаблед</strong></a><br /> | Только для чтения<br /> | Указывает, доступен ли интерфейс <a href="imstscsecuredsettings-interface.md"><strong>имстсксекуредсеттингс</strong></a> .<br /> | 
| <a href="imstscax-server.md"><strong>Сервером</strong></a><br /> | Чтение/запись<br /> | Имя сервера, к которому подключен текущий элемент управления.<br /> | 
| <a href="imsrdpclientnonscriptable3-showredirectionwarningdialog.md"><strong>шовредиректионварнингдиалог</strong></a><br /> | Чтение/запись<br /> | Указывает, следует ли отображать диалоговое окно предупреждения безопасности перенаправления перед запуском сеанса.<br /> | 
| <a href="imstscax-startconnected.md"><strong>стартконнектед</strong></a><br /> | Чтение/запись<br /> | Указывает, будет ли элемент управления устанавливать соединение с сервером узла сеансов удаленных рабочих столов сразу после запуска.<br /> | 
| <a href="imsrdpclient5-transportsettings.md"><strong>TransportSettings</strong></a><br /> | Только для чтения<br /> | Параметр шлюза клиентских удаленных рабочих столов.<br /> | 
| <a href="imsrdpclientnonscriptable2-uiparentwindowhandle.md"><strong>уипарентвиндовхандле</strong></a><br /> | Чтение/запись<br /> | Маркер окна, который будет родительским окном для элемента управления. Это позволяет корректно модальным окнам, отображаемым элементом управления, по отношению к любым окнам, отображаемым родительским приложением.<br /> | 
| <a href="imstscax-username.md"><strong>Имен</strong></a><br /> | Чтение/запись<br /> | Учетные данные имени пользователя для входа.<br /> | 
| <a href="imstscax-version.md"><strong>Версия</strong></a><br /> | Только для чтения<br /> | Номер версии текущего элемента управления.<br /> | 
| <a href="imstscax-verticalscrollbarvisible.md"><strong>вертикалскроллбарвисибле</strong></a><br /> | Только для чтения<br /> | Указывает, отображает ли элемент управления вертикальную полосу прокрутки.<br /> | 
| <a href="imsrdpclientnonscriptable3-warnaboutclipboardredirection.md"><strong>варнабаутклипбоардредиректион</strong></a><br /> | Чтение/запись<br /> | Указывает, должно ли диалоговое окно "предупреждение системы безопасности" включать предупреждение о перенаправлении буфера обмена перед запуском сеанса.<br /> | 
| <a href="imsrdpclientnonscriptable3-warnaboutsendingcredentials.md"><strong>варнабаутсендингкредентиалс</strong></a><br /> | Чтение/запись<br /> | Указывает, должно ли предупреждение безопасности включать предупреждение об отправке учетных данных на удаленный сервер перед запуском сеанса.<br /> | 




 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                             |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                                       |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>               |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>               |
| CLSID<br/>                    | \_MSRDPCLIENT5NOTSAFEFORSCRIPTING CLSID определен как 4EB2F086-C818-447E-B32C-C51CE2B30D31<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[удаленный рабочий стол классы элементов управления ActiveX](remote-desktop-activex-control-classes.md)
</dt> </dl>

 

