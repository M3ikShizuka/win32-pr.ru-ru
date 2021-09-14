---
description: Слабо связанный Internet Explorer (ЛЦИЕ) повышает надежность обозревателя за счет разделения компонентов и ослабления их взаимозависимости.
ms.assetid: 7609090E-7E2B-4B1F-80FF-192B30A40244
title: архитектура (Windows 7 и Windows Server 2008 R2 Quality Cookbook)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6edd27246b7b19765288a280bd467de86d2fe50f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127249394"
---
# <a name="architecture-windows-7-and-windows-server-2008-r2-application-quality-cookbook"></a>архитектура (Windows 7 и Windows Server 2008 R2 Quality Cookbook)

*Слабо связанный Internet Explorer* (лЦие) повышает надежность обозревателя за счет разделения компонентов и ослабления их взаимозависимости.

в частности, лЦие пытается изолировать Windows фрейм Internet Explorer и его вкладки в отдельных процессах. в Windows Internet Explorer 8 такая изоляция повышает производительность и масштабируемость. это изменение архитектуры может повлиять на совместимость расширений и надстроек, включая ActiveX элементы управления, вспомогательные объекты браузера (bho) и компоненты панели инструментов пользовательского интерфейса, созданные с помощью старых методов программирования.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Разработка обновлений, влияющих на совместимость браузеров](design-updates-that-impact-compatibility-between-browsers.md)
</dt> </dl>

 

 



