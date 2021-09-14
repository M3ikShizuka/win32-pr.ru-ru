---
description: Демонстрирует, как реализовать команду оболочки с помощью методов Експлореркомманд и Експлореркоммандстате.
title: 'Пример: команда в проводнике'
ms.topic: article
ms.date: 05/31/2018
ms.assetid: 2310A6AA-EAF9-4d7a-A784-04931BDC2089
api_name: ''
api_type: ''
api_location: ''
topic_type:
- kbArticle
ms.openlocfilehash: a35662c3df0e0fcddae049ccfaac2d9e3e265ee3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127248035"
---
# <a name="explorer-command-verb-sample"></a>Пример: команда в проводнике

Демонстрирует, как реализовать команду оболочки с помощью методов Експлореркомманд и Експлореркоммандстате.

В этом разделе содержатся следующие подразделы.

-   [Requirements](#requirements)
-   [Загрузка образца](#downloading-the-sample)
-   [Создание примера](#building-the-sample)
-   [Запуск примера](#running-the-sample)

## <a name="requirements"></a>Требования



| Продукт                                | Минимальная версия продукта |
|----------------------------------------|-------------------------|
| Windows                                | Windows Vista           |
| Windows SDK | 7.0                     |



 

## <a name="downloading-the-sample"></a>Загрузка образца

| Расположение      | URL-адрес пути                                                                                             |
|---------------|------------------------------------------------------------------------------------------------------|
| GitHub  | [Пример Експлореркоммандверб](https://github.com/microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/shell/appshellintegration/ExplorerCommandVerb) |

## <a name="building-the-sample"></a>Построение образца

Чтобы построить образец из командной строки, выполните следующую команду:

1.  Откройте окно командной строки и перейдите в каталог проекта **експлореркоммандверб** .
2.  Введите `msbuild ExplorerCommandVerb.sln`.

чтобы создать пример с использованием Microsoft Visual Studio (предпочтительно):

1.  откройте обозреватель Windows и перейдите в каталог проекта **експлореркоммандверб** .
2.  Дважды щелкните значок файла Експлореркоммандверб. sln, чтобы открыть проект в Visual Studio.
3.  В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1.  перейдите в каталог, содержащий ExplorerCommandVerb.dll, используя командную строку или обозреватель Windows. Убедитесь, что используется 64-разрядный файл DLL на 64-разрядной Windows.
2.  В командной строке введите `regsvr32.exe ExplorerCommandVerb.dll` .
3.  Если щелкнуть правой кнопкой мыши файл .txt, в контекстном меню будут отображаться две новые команды.

 

 



