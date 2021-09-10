---
title: Функции обратного вызова yield
description: Функции обратного вызова yield
ms.assetid: 8c9b43ea-fdba-41a2-ba2d-1eaa4516e14f
keywords:
- Функции обратного вызова Авикап, yield
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3666ea24a1d37402ffc13c09ca8ab95fcd19e1f7
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124372561"
---
# <a name="yield-callback-functions"></a>Функции обратного вызова yield

Приложения могут использовать функцию yield callback во время потоковой записи. (Функция обратного вызова, как правило, состоит из цикла обработки сообщений, который вызывает [PeekMessage](/windows/win32/api/winuser/nf-winuser-peekmessagea), [TranslateMessage](/windows/win32/api/winuser/nf-winuser-translatemessage)и [DispatchMessage](/windows/win32/api/winuser/nf-winuser-dispatchmessage).) Окно Capture вызывает функцию обратного вызова yield по крайней мере один раз для каждого захваченного видеокадра, но Точная скорость зависит от частоты кадров и нагрузки на диск и драйвер записи.

 

 