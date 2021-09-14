---
title: Преобразование в JavaScript из JScript
description: Преобразование в JavaScript из JScript
ms.assetid: 11d31c8c-868d-4220-9298-6d24a209dc47
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 71b18972f407cf008626245798b3f7740d98058e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127253060"
---
# <a name="translating-to-javascript-from-jscript"></a>Преобразование в JavaScript из JScript

JScript в значительной степени совместима с JavaScript. однако JScript содержит некоторые объекты, которые в настоящее время не поддерживаются JavaScript, такие как активексобжект, Enumerator, Error, Global и VBArray.

JScript версии 5,0 поддерживает обработку исключений с помощью **try**... операторы **catch** . В настоящее время JavaScript не предоставляет механизм обработки ошибок.

при работе с JScript или JavaScript существует ряд незначительных различий между реализациями объектной модели, поддерживаемыми различными веб-браузерами. Чтобы написать сценарий, выполняемый как в Internet Explorer, так и в Netscape Navigator, ограничьте функции, используемые скриптами, указанными в стандарте консорциум W3C (W3C) [для HTML версии 3,2](https://www.w3.org/tr/rec-html32.html).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Преобразование в JavaScript](translating-to-javascript.md)
</dt> </dl>

 

 




