---
title: Флаг теста
description: Флаг теста
ms.assetid: d103a96e-8d55-413d-ac84-15c3d8dccfbe
keywords:
- Флаг MCI_TEST
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2a36cddaa186a9be260cf87b7a323a6e05ed9fc4
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371562"
---
# <a name="the-test-flag"></a>Флаг теста

Флаг Test ( \_ тест MCI) выполняет запрос устройства, чтобы определить, может ли он выполнить команду. Устройство возвращает ошибку, если не может выполнить команду. Он не возвращает ошибку, если может справиться с командой. При указании этого флага MCI возвращает управление приложению, не выполняя команду.

Этот флаг поддерживается устройствами цифрового видео и ВИДЕОМАГНИТОФОНА для всех команд, кроме [**Open**](open.md) ([**MCI \_ Open**](mci-open.md)) и [**Close**](close.md) ([**MCI \_ Close**](mci-close.md)).

 

 




