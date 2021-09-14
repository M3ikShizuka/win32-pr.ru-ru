---
description: Демонстрирует использование \_ интерфейсов API командной консоли NotifyIcon и оболочки \_ нотификонжетрект для отображения значка уведомления.
title: Пример NotificationIcon
ms.topic: article
ms.date: 05/31/2018
ms.assetid: 9F31DB2D-4B12-4f65-AC91-25B4B5B1CB46
api_name: ''
api_type: ''
api_location: ''
topic_type:
- kbArticle
ms.openlocfilehash: 1569d162aef358130910081bee80354cb64f690d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343587"
---
# <a name="notificationicon-sample"></a>Пример NotificationIcon

Демонстрирует использование интерфейсов API [**командной консоли \_ NotifyIcon**](/windows/desktop/api/Shellapi/nf-shellapi-shell_notifyicona) и [**оболочки \_ нотификонжетрект**](/windows/desktop/api/Shellapi/nf-shellapi-shell_notifyicongetrect) для отображения значка уведомления.

В этом разделе содержатся следующие подразделы.

-   [Описание](#description)
-   [Requirements](#requirements)
-   [Загрузка образца](#downloading-the-sample)
-   [Создание примера](#building-the-sample)
-   [Запуск примера](#running-the-sample)

## <a name="description"></a>Описание

Кроме того, чтобы отобразить значок уведомления, в этом примере также демонстрируется отображение форматированного всплывающего окна, контекстного меню и всплывающего уведомления в дополнение к использованию [**оболочки \_ NotifyIcon**](/windows/desktop/api/Shellapi/nf-shellapi-shell_notifyicona) и [**\_ нотификонжетрект оболочки**](/windows/desktop/api/Shellapi/nf-shellapi-shell_notifyicongetrect) .

> [!Note]  
> [**Оболочка \_ нотификонжетрект**](/windows/desktop/api/Shellapi/nf-shellapi-shell_notifyicongetrect) доступен только в Windows 7 и более поздних версиях.

 

## <a name="requirements"></a>Требования



| Продукт                                | Минимальная версия продукта |
|----------------------------------------|-------------------------|
| Windows                                | Windows 7               |
| Windows SDK | 7.0                     |



 

## <a name="downloading-the-sample"></a>Загрузка образца

| Расположение      | URL-адрес пути                                                                                             |
|---------------|------------------------------------------------------------------------------------------------------|
| GitHub  | [Пример Нотификатионикон](https://github.com/microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/winui/shell/appshellintegration/NotificationIcon) |

## <a name="building-the-sample"></a>Построение образца

Чтобы построить образец из командной строки, выполните следующую команду:

1.  Откройте окно командной строки и перейдите в каталог проекта **нотификатионикон** .
2.  Введите `msbuild NotificationIcon.sln`.

чтобы создать пример с использованием Microsoft Visual Studio (предпочтительно):

1.  откройте обозреватель Windows и перейдите в каталог проекта **нотификатионикон** .
2.  Дважды щелкните значок файла Нотификатионикон. sln, чтобы открыть проект в Visual Studio.
3.  В меню **Построение** выберите пункт **Построить решение**.

## <a name="running-the-sample"></a>Запуск примера

1.  перейдите в каталог, содержащий новый исполняемый файл, используя командную строку или обозреватель Windows.
2.  В командной строке введите `NotificationIcon.exe` . кроме того, в обозревателе Windows дважды щелкните значок NotificationIcon.exe.

> [!Note]  
> Значки уведомлений, заданные с помощью идентификатора GUID, защищаются от подмены путем проверки того, что они регистрируются только одним приложением. Эта регистрация выполняется при первом вызове оболочки \_ NotifyIcon (ним \_ Add,...) и сохранении полного пути вызывающего приложения. Если позже вы переместит двоичный файл в другое расположение, система не разрешит добавить значок снова. Дополнительные сведения см. в разделе [**оболочка \_ NotifyIcon**](/windows/desktop/api/Shellapi/nf-shellapi-shell_notifyicona) .

 

 

 



