---
title: Удаленное управление Windows
description: Windows удаленное управление (служба удаленного управления Windows) — это реализация WS-Management протокола майкрософт стандартного протокола на основе SOAP, обеспечивающего взаимодействие оборудования и операционных систем от разных поставщиков.
ms.assetid: 6429e748-e0bf-431a-8989-db5b211665d5
ms.tgt_platform: multiple
keywords:
- Windows Удаленное управление (WinRM), начальная страница
- WS-Management
ms.topic: article
ms.date: 09/10/2021
topic_type:
- kbOrient
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: b0744e5ad50ac602071a946dab76a864684d7b60
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126974802"
---
# <a name="windows-remote-management"></a>Удаленное управление Windows

## <a name="what-is-winrm"></a>Что такое WinRM?

С помощью удаленного управления Windows (WinRM) корпорация Майкрософт реализует стандартный [протокол WS-Management](ws-management-protocol.md), основанный на протоколе SOAP. Он удобен для брандмауэров и обеспечивает взаимодействие оборудования и операционных систем различных поставщиков.

Спецификация протокола WS-Management предоставляет системам общий способ доступа и обмена данными управления в ИТ-инфраструктуре. WinRM и [*интеллектуальный интерфейс управления платформой (IPMI)*](windows-remote-management-glossary.md#i)вместе с [сборщиком событий](/previous-versions/windows/it-pro/windows-server-2003/cc785056(v=ws.10)#event-collector) являются компонентами компонентов [Windows аппаратного управления](/previous-versions/windows/it-pro/windows-server-2003/cc785056(v=ws.10)) .

## <a name="where-can-i-use-winrm"></a>Где можно использовать WinRM?

для получения данных управления с локальных и удаленных компьютеров, на которых могут использоваться [*контроллеры управления основной платой (bmc)*](windows-remote-management-glossary.md), можно использовать объекты скриптов winrm, программу командной строки winrm или средство командной строки Windows удаленной оболочки. если компьютер работает под управлением Windows версии операционной системы, включающей WinRM, данные управления передаются [инструментарий управления Windows (WMI) (WMI)](/windows/desktop/WmiSdk/wmi-start-page).

Данные об оборудовании и системе также можно получить из реализаций протокола WS-Management, работающих в других операционных системах (не Windows) на предприятии. WinRM устанавливает сеанс связи с другим компьютером по протоколу WS-Management на основе SOAP, а не подключается через DCOM, как WMI. Данные возвращаются протоколу WS-Management в формате XML, а не в виде объектов.

Поставщик [IPMI](/previous-versions/windows/desktop/ipmiprv/ipmi-provider) WMI — это стандартный поставщик WMI с классами, получающими данные датчика BMC с компьютеров с соответствующим оборудованием. Доступ к данным IPMI можно получить с помощью API-интерфейсов WinRM, [скриптов](/windows/desktop/WmiSdk/scripting-api-for-wmi)WMI или [com](/windows/desktop/WmiSdk/com-api-for-wmi) .

## <a name="who-is-this-for"></a>Кто это для?

предполагаемая аудитория для служба удаленного управления Windows — ит-специалисты, которые пишут сценарии для автоматизации управления серверами, а также независимые разработчики программного обеспечения, желающие получить данные для приложений управления.

## <a name="run-time-requirements"></a>Требования к среде выполнения

WinRM является частью операционной системы. Однако для получения данных с удаленных компьютеров необходимо настроить [*прослушиватель*](windows-remote-management-glossary.md#l)WinRM. дополнительные сведения см. в разделе [установка и настройка для служба удаленного управления Windows](installation-and-configuration-for-windows-remote-management.md). Если контроллер BMC обнаруживается при запуске системы, поставщик IPMI загружается; в противном случае объекты скриптов WinRM и средство командной строки WinRM остаются доступными.

## <a name="learn-more"></a>Подробнее

[о служба удаленного управления Windows](about-windows-remote-management.md)

Ссылка на общедоступную спецификацию протокола WS-Management, архитектуру WinRM, связь с WMI, управление оборудованием с помощью поставщика IPMI, конфигурации и установки.

[использование служба удаленного управления Windows](using-windows-remote-management.md)

Приступая к работе с API-интерфейсом WinRM Scripting и аппаратным управлением.

[Windows Справочник по удаленному управлению](windows-remote-management-reference.md)

Список интерфейсов сценариев, определенных веб-службами Майкрософт для автоматизации управления (WS-Management) и определений классов классов WMI, созданных поставщиком IPMI и классами, взаимодействующими с драйвером IPMI для получения данных [контроллера управления основной платой (BMC)](windows-remote-management-glossary.md) .
