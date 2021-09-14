---
description: В этом разделе описываются технологии документов, поддерживаемые Microsoft Windows.
ms.assetid: 14ae2c97-8596-46db-a55c-ef706d2cd00b
title: XPS-документы
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 625c2f04a43db9433fe125b52a4bbc08e37fb4f4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343683"
---
# <a name="xps-documents"></a>XPS-документы

В этом разделе описываются технологии документов, поддерживаемые Microsoft Windows.

-   [Выбор технологии документов](#choosing-a-document-technology)
-   [В этом разделе](#in-this-section)
-   [Средства документов XPS](#xps-document-tools)
-   [Связанные темы](#related-topics)


## <a name="choosing-a-document-technology"></a>Выбор технологии документов

Корпорация Майкрософт предоставляет несколько различных технологий документов для поддержки различных приложений для работы с документами:

-   **XPS и Опенкспс**

    в Windows 8 и более поздних версиях Windows поддерживаются XPS и опенкспс. Чтобы определить правильный сценарий использования для XPS и Опенкспс, см. предыдущую схему. Дополнительные сведения об этих технологиях документов см. в [статье Спецификация Open XML Paper (опенкспс)](https://www.ecma-international.org/publications/standards/Ecma-388.htm).

    в случае использования опенкспс с Windows 8 и Windows Server 2012, поддержка предоставляется только через [API документов XPS](documents-xps.md) .

    Если необходимо выполнить преобразование между Microsoft XPS (МСКСПС) и Опенкспс, то корпорация Майкрософт предоставила средство (XPSConverter.exe), которое позволяет преобразовать документы МСКСПС в формат Опенкспс и наоборот. средство входит в комплект Windows Driver Kit (WDK). Чтобы скачать WDK, см. статью [как получить WDK](/windows-hardware/drivers/download-the-wdk).

    дополнительные сведения о опенкспс и Windows 8 см. в разделе [поддержка опенкспс в Windows](/windows-hardware/drivers/print/driver-support-for-openxps).

-   **API документов XPS**

    api документов xps — это собственный интерфейс api Windows, поддерживающий OM-элемент xps. API документов XPS появился в Windows 7 и может использоваться в программах пользовательского режима и драйверах принтера XPSDrv.

    Дополнительные сведения см. в статье API документов XPS и [API цифровой подписи XPS](xps-digital-signatures.md).

    \*API документов XPS также поддерживается в Windows Vista с пакетом обновления 2 (sp2) с обновлением платформы для Windows Vista и Windows Server 2008 с пакетом обновления 2 (sp2) с обновлением платформы для Windows server 2008. дополнительные сведения об обновлении платформы для Windows vista или обновления платформы для Windows Server 2008 см. в [статье обновление платформы для Windows vista](/windows/desktop/win7ip/platform-update-for-windows-vista-portal) .

-   **.NET Framework**

    платформа .NET Framework обеспечивает поддержку документов XPS для программ, управляемых в пользовательском режиме.

    платформа .NET Framework 3,0 поддерживается в Windows XP с пакетом обновления 2 (sp2) и более поздних версиях Windows клиентских операционных систем, а также на Windows server 2003 с пакетом обновления 2 (sp2) и более поздних версиях операционных систем Windows Server.

    платформа .NET Framework 3,5 поддерживается в Windows клиентских операционных системах Windows XP и в Windows server 2003 и более поздних версиях Windows серверных операционных систем.

    > [!Note]  
    > рекомендуется использовать платформа .NET Framework для создания документов XPS только в клиентских приложениях, а не в серверных приложениях, если приложение не будет периодически завершать работу, как если бы оно было клиентским приложением.

     

    дополнительные сведения о поддержке документов в платформа .NET Framework см. в разделе [Windows Presentation Foundation документы](/previous-versions/dotnet/netframework-3.0/ms749165(v=vs.85)).

> [!Note]  
> для работы с XPS-документами в программе используйте собственный API документа xps или платформа .NET Framework. одновременное использование обоих в одной программе не поддерживается.

 

## <a name="in-this-section"></a>в этом разделе

в этом разделе описаны технологии документов машинного Windows, поддерживаемые Microsoft Windows.



| Технология документов                                                                   | Описание                                                                                                                                                                                                                                |
|--------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [API документов XPS](documents-xps.md)<br/>                   | Предоставляет надежный формат для электронной бумаги.<br/> API документа XPS, описанный в этом разделе, предоставляет программам и драйверам печати доступ к содержимому и метаданным документа XPS.<br/> |
| [API цифровой подписи XPS](xps-digital-signatures.md)<br/> | Включает подписывание документов, проверку удостоверения подписавшего и указывает, изменился ли документ XPS с момента подписания.<br/>                                                                          |
| [Глоссарий XPS-документов](xpsapi-glossary.md)<br/>           | Определения терминов, используемых [API документов XPS](documents-xps.md) и [API цифровой подписи XPS](xps-digital-signatures.md).<br/>                                                                              |



 

## <a name="xps-document-tools"></a>Средства документов XPS

Доступны следующие средства для тестирования и устранения неполадок в файлах XPS-документов.

-   [IsXPS](/previous-versions/aa348104(v=vs.110))

    Проверяет соответствие файла спецификациям формата XML (XPS) и спецификации Open Packaging Conventions (OPC).

-   [кспсанализер](/windows-hardware/drivers/devtest/xpsanalyzer)

    Средство командной строки, которое анализирует файлы документов XPS на совместимость со спецификацией XPS 1,0.

-   [птконформ](/previous-versions/dd327476(v=msdn.10))

    Средство, проверяющее допустимость документов PrintTicket и PrintCapabilities.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[API печати XPS](./printing-with-the-xpsprint-api.md)
</dt> <dt>

[Упаковка](/previous-versions/windows/desktop/opc/packaging)
</dt> <dt>

[Вывод на печать](./printdocs-printing.md)
</dt> <dt>
  
[Пример программы печати](https://github.com/microsoftarchive/msdn-code-gallery-microsoft/tree/master/Official%20Windows%20Platform%20Sample/Windows%208%20app%20samples/%5BC%2B%2B%5D-Windows%208%20app%20samples/C%2B%2B/Windows%208%20app%20samples/Print%20sample%20(Windows%208))
</dt> </dl>

 

