---
title: преобразование в JScript из JavaScript
description: преобразование в JScript из JavaScript
ms.assetid: 86067a69-a6a1-474f-b8d8-85caf384a311
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 45535807a5ef2baf59c2e068007a5a8df8bf4863
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571894"
---
# <a name="translating-to-jscript-from-javascript"></a>преобразование в JScript из JavaScript

JScript в значительной степени совместима с JavaScript. однако JScript версии 5,0 включает в себя некоторые объекты, которые в настоящее время не поддерживаются JavaScript, такие как активексобжект, Enumerator, Error, Global и VBArray.

JScript 5,0 поддерживает обработку исключений с помощью **try**... операторы **catch** . В настоящее время JavaScript не предоставляет механизм обработки ошибок.

при работе с JScript или JavaScript существует ряд незначительных различий между реализациями объектной модели, поддерживаемыми различными веб-браузерами. Чтобы написать сценарий, выполняемый как в Internet Explorer, так и в Netscape Navigator, ограничьте функции, используемые скриптами, указанными в стандарте консорциум W3C (W3C) для HTML версии 3,2. Дополнительные сведения об этом стандарте см. в разделе [эталонная спецификация HTML 3,2](https://www.w3.org/TR/REC-html32.html).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Перевод в JScript](translating-to-jscript.md)
</dt> </dl>

 

 




