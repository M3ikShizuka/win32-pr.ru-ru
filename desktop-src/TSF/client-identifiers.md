---
title: Идентификаторы клиентов
description: Идентификаторы клиентов
ms.assetid: 69ff159c-9264-4958-a712-4aa50db6e48e
keywords:
- Платформа текстовых служб (TSF), идентификаторы клиентов
- TSF (платформа текстовых служб), идентификаторы клиентов
- текстовые службы, идентификаторы клиентов
- Приложения с поддержкой TSF, идентификаторы клиентов
- идентификаторы клиентов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9de15b208d2fbc6c6ea5c2a1114eb5cb23ff12ff
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243712"
---
# <a name="client-identifiers"></a>Идентификаторы клиентов

## <a name="applications"></a>Приложения

Приложение получает свой идентификатор клиента путем вызова [ITfThreadMgr:: Activate](/windows/desktop/api/Msctf/nf-msctf-itfthreadmgr-activate).

## <a name="text-services"></a>Текстовые службы

Служба текстового ввода получает свой идентификатор клиента при вызове метода [итфтекстинпутпроцессор:: Activate](/windows/desktop/api/Msctf/nf-msctf-itftextinputprocessor-activate) текстовой службы.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[ITfThreadMgr:: Activate](/windows/desktop/api/Msctf/nf-msctf-itfthreadmgr-activate)
</dt> <dt>

[Итфтекстинпутпроцессор:: Activate](/windows/desktop/api/Msctf/nf-msctf-itftextinputprocessor-activate)
</dt> </dl>

 

 




