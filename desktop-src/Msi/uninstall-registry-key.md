---
description: список свойств установщик Windows, предоставляя значения, записанные в разделе реестра Uninstall.
ms.assetid: f831cc62-4b19-4285-8bb1-6080567ac985
title: Windows Свойства установщика для раздела реестра Uninstall
ms.topic: article
ms.date: 05/31/2018
ms.custom: contperf-fy21q3
ms.openlocfilehash: 90174cabed7a1d9ff0ca21b532c459a1026787a6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171620"
---
# <a name="windows-installer-properties-for-the-uninstall-registry-key"></a>Windows Свойства установщика для раздела реестра Uninstall

Следующие свойства установщика предоставляют значения, записываемые в раздел реестра:

**HKey \_ \_** \\ **программное обеспечение** локального компьютера ( \\ **Microsoft** \\ **Windows** \\ **CurrentVersion** \\  )

Значения хранятся в подразделе, определяемом идентификатором GUID кода продукта приложения.



| Значение               | Windows Свойство установщика                                                                                                                                                                                                                                                                                                                                           |
|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DisplayName         | Свойство [**ProductName**](productname.md)                                                                                                                                                                                                                                                                                                                          |
| DisplayVersion      | Производный от свойства [**ProductVersion**](productversion.md)                                                                                                                                                                                                                                                                                                       |
| Publisher           | Свойство [**Manufacturer**](manufacturer.md)                                                                                                                                                                                                                                                                                                                        |
| VersionMinor        | Производный от свойства [**ProductVersion**](productversion.md)                                                                                                                                                                                                                                                                                                       |
| VersionMajor        | Производный от свойства [**ProductVersion**](productversion.md)                                                                                                                                                                                                                                                                                                       |
| Версия             | Производный от свойства [**ProductVersion**](productversion.md)                                                                                                                                                                                                                                                                                                       |
| HelpLink            | [**Арфелплинк**](arphelplink.md) , свойство                                                                                                                                                                                                                                                                                                                          |
| хелптелефоне       | [**Арфелптелефоне**](arphelptelephone.md) , свойство                                                                                                                                                                                                                                                                                                                |
| InstallDate         | Время последнего поступления этого продукта в службу. Значение этого свойства заменяется каждый раз, когда к продукту применяется или удаляется исправление, или для восстановления продукта используется [параметр командной строки](command-line-options.md) /v. Если продукт не получил исправлений или обновлений, это свойство содержит время установки продукта на этом компьютере. |
| InstallLocation     | [**Арпинсталллокатион**](arpinstalllocation.md) , свойство                                                                                                                                                                                                                                                                                                            |
| инсталлсаурце       | [**SourceDir**](sourcedir.md) , свойство                                                                                                                                                                                                                                                                                                                              |
| урлинфоабаут        | [**Арпурлинфоабаут**](arpurlinfoabout.md) , свойство                                                                                                                                                                                                                                                                                                                  |
| урлупдатеинфо       | [**Арпурлупдатеинфо**](arpurlupdateinfo.md) , свойство                                                                                                                                                                                                                                                                                                                |
| аусоризедкдфпрефикс | [**Арпаусоризедкдфпрефикс**](arpauthorizedcdfprefix.md) , свойство                                                                                                                                                                                                                                                                                                    |
| Комментарии            | [**Арпкомментс**](arpcomments.md) , свойство <br/> Комментарии, указанные на панели управления " **Установка и удаление программ** ".<br/>                                                                                                                                                                                                                                |
| Contact             | [**Арпконтакт**](arpcontact.md) , свойство <br/> Обратитесь к панели управления **Установка и удаление программ** .<br/>                                                                                                                                                                                                                                   |
| EstimatedSize       | определяется и задается установщик Windows.                                                                                                                                                                                                                                                                                                                         |
| Язык            | [**Продуктлангуаже**](productlanguage.md) , свойство                                                                                                                                                                                                                                                                                                                  |
| модифипас          | определяется и задается установщик Windows.                                                                                                                                                                                                                                                                                                                         |
| Readme              | [**Арпреадме**](arpreadme.md) , свойство <br/> Файл readme, указанный на панели управления " **Установка и удаление программ** ".<br/>                                                                                                                                                                                                                                      |
| UninstallString     | определяется и задается установщик Windows.                                                                                                                                                                                                                                                                                                                             |
| сеттингсидентифиер  | [**Мсиарпсеттингсидентифиер**](msiarpsettingsidentifier.md) , свойство                                                                                                                                                                                                                                                                                                |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сведения о свойствах](about-properties.md)
</dt> <dt>

[настройка установки и удаления программ с помощью установщик Windows](configuring-add-remove-programs-with-windows-installer.md)
</dt> <dt>

[Справочник по свойствам](property-reference.md)
</dt> <dt>

[Использование свойств](using-properties.md)
</dt> </dl>

 

 




