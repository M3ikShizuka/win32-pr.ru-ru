---
title: настройка Потоки скриптов
description: настройка Потоки скриптов
ms.assetid: f8f1656e-69c6-47f7-a8eb-c1039a84ebf3
keywords:
- потоки, Настройка потоков скриптов
- кодеки, Настройка потоков сценариев
- Создание скриптов для потоков, Настройка
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e063865b301c8c7c2a4171aa530a89464306c0ad
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127251533"
---
# <a name="configuring-script-streams"></a>настройка Потоки скриптов

Как и для всех произвольных типов потоков, потоки сценариев должны иметь определенную скорость потока и окно буфера. Основной тип носителя в структуре [**\_ \_ типа мультимедиа WM**](/previous-versions/windows/desktop/api/wmsdkidl/ns-wmsdkidl-wm_media_type) должен быть установлен в вммедиатипе \_ script.

Для потоков сценариев необходимо, чтобы член **форматтипе** **\_ \_ типа мультимедиа WM** был установлен в вмформат \_ скрипт, который указывает, что элемент **пбформат** указывает на структуру [**вмскриптформат**](/previous-versions/windows/desktop/api/wmsdkidl/ns-wmsdkidl-wmscriptformat) .

Существует только один поддерживаемый тип скрипта, ВМСКРИПТТИПЕ \_ твострингс.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**общая конфигурация для всех Потоки**](configuration-common-to-all-streams.md)
</dt> <dt>

[**Настройка произвольных типов потоков**](configuring-arbitrary-stream-types.md)
</dt> <dt>

[**Команды скриптов**](script-commands.md)
</dt> </dl>

 

 




