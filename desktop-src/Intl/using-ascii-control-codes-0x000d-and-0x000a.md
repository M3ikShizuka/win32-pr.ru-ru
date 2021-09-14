---
description: Стандарт Unicode не предписывает определенные значения для управляющих кодов 0x000D (возврат каретки) и 0x000A (перевод строки).
ms.assetid: fb8b1a5c-79a4-45a0-b7a1-8217c370d13e
title: Использование управляющих кодов ASCII 0x000D и 0x000A
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d509c83bfd6349dcceb05ab4a8946aae51feacdc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254911"
---
# <a name="using-ascii-control-codes-0x000d-and-0x000a"></a>Использование управляющих кодов ASCII 0x000D и 0x000A

Стандарт Unicode не предписывает определенные значения для управляющих кодов 0x000D (возврат каретки) и 0x000A (перевод строки). Эти коды не обязательно использовать в сочетании. Если используется по отдельности, либо код может представлять только себя, либо оба кода вместе. Приложение должно всегда определять, что представляют эти коды.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование специальных символов в Юникоде](using-special-characters-in-unicode.md)
</dt> </dl>

 

 



