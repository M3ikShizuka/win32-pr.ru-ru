---
description: MsiFiler.exe заполняет таблицу файлов версиями, языками и размерами на основе исходного каталога. Также можно обновить таблицу Мсифилехаш с помощью хэшей файлов.
ms.assetid: cc3db60b-0b1d-4582-8b40-0b55f83e00be
title: Msifiler.exe
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b2d7aeceae7abd8a9786079788e68c7d7bda35ae
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065310"
---
# <a name="msifilerexe"></a>Msifiler.exe

MsiFiler.exe заполняет [таблицу файлов](file-table.md) версиями, языками и размерами на основе исходного каталога. Также можно обновить [таблицу мсифилехаш](msifilehash-table.md) с помощью хэшей файлов.

## <a name="syntax"></a>Синтаксис

**msifiler.exe-d** *{Database}* **\[ -v \] \[ -h \] \[ -s алтсаурце \]**

## <a name="command-line-options"></a>Параметры командной строки

В Msifiler.exe используются следующие параметры командной строки без учета регистра. Вместо тире можно использовать разделитель с косой чертой.



| Параметр | Параметр   | Описание                                                                                                                                                                  |
|--------|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| -d     | *database*  | База данных (файл .msi), которую требуется обновить.                                                                                                                              |
| -v     |             | Использовать режим подробного вывода.                                                                                                                                                            |
| -H     |             | Заполнение [таблицы мсифилехаш](msifilehash-table.md). При этом создается таблица, если она еще не существует. Таблицу Мсифилехаш можно использовать только с файлами без версий. |
| -S     | *алтсаурце* | АЛТСАУРЦЕ указывает альтернативный каталог для поиска файлов.                                                                                                              |



 

это средство доступно только в [компонентах Windows SDK для разработчиков установщик Windows](platform-sdk-components-for-windows-installer-developers.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Windows Средства разработки установщика](windows-installer-development-tools.md)
</dt> <dt>

[Использование таблицы Directory](using-the-directory-table.md)
</dt> <dt>

[Выпущенные версии, средства и распространяемые пакеты](released-versions-tools-and-redistributables.md)
</dt> </dl>

 

 



