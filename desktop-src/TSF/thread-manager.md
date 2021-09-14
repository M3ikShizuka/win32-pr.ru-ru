---
title: Диспетчер потоков
description: Диспетчер потоков является базовым компонентом диспетчера TSF.
ms.assetid: fd43b4c3-80bb-4118-a880-bdea07022c95
keywords:
- Платформа текстовых служб (TSF), диспетчер потоков
- TSF (платформа текстовых служб), диспетчер потоков
- текстовые службы, диспетчер потоков
- Приложения с поддержкой TSF, диспетчер потоков
- Диспетчер потоков
- Диспетчер TSF
- уведомления о событиях
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4b29596c5c39267181c6a2c301aede3f15ca7297
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056760"
---
# <a name="thread-manager"></a>Диспетчер потоков

Диспетчер потоков является базовым компонентом диспетчера TSF. Диспетчер потоков выполняет стандартные задачи, связанные с приложениями и текстовыми службами (клиентами). Эти задачи включают, но не ограничиваются, активацию и деактивацию текстовых служб TSF, создание диспетчеров документов и обслуживание правильной связи между документами и фокусом ввода. Диспетчер потоков определяется интерфейсом [ITfThreadMgr](/windows/desktop/api/Msctf/nn-msctf-itfthreadmgr) .

Большинство интерфейсов и объектов, предоставляемых диспетчером TSF, можно получить с помощью методов, предоставляемых интерфейсом диспетчера потоков.

## <a name="applications"></a>Приложения

Приложение создает объект диспетчера потоков путем вызова [CoCreateInstance](/windows/win32/api/combaseapi/nf-combaseapi-cocreateinstance) с помощью CLSID \_ тфсреадмгр.

## <a name="text-services"></a>Текстовые службы

Служба текстового ввода получает объект диспетчера потоков в метод Text службы [итфтекстинпутпроцессор:: Activate](/windows/desktop/api/Msctf/nf-msctf-itftextinputprocessor-activate) .

## <a name="event-notifications"></a>Уведомления о событиях

Диспетчер потоков также предоставляет клиентам уведомления о событиях. В TSF уведомления о событиях предоставляются с помощью приемника событий, который является COM-объектом. Чтобы получать уведомления от диспетчера потоков, клиент реализует объект [итфсреадмгревентсинк](/windows/desktop/api/Msctf/nn-msctf-itfthreadmgreventsink) и устанавливает приемник событий. Приемник событий устанавливается путем запроса диспетчера потоков для IID \_ итфсаурце и вызова [итфсаурце:: ADVISESINK](/windows/desktop/api/Msctf/nf-msctf-itfsource-advisesink) с IID \_ итфсреадмгревентсинк.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[ITfThreadMgr](/windows/desktop/api/Msctf/nn-msctf-itfthreadmgr)
</dt> <dt>

[CoCreateInstance](/windows/win32/api/combaseapi/nf-combaseapi-cocreateinstance)
</dt> <dt>

[Итфтекстинпутпроцессор:: Activate](/windows/desktop/api/Msctf/nf-msctf-itftextinputprocessor-activate)
</dt> <dt>

[итфсреадмгревентсинк](/windows/desktop/api/Msctf/nn-msctf-itfthreadmgreventsink)
</dt> <dt>

[Итфсаурце:: AdviseSink](/windows/desktop/api/Msctf/nf-msctf-itfsource-advisesink)
</dt> </dl>

 

 