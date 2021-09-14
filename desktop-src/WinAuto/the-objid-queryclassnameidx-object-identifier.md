---
title: Идентификатор объекта OBJID_QUERYCLASSNAMEIDX
description: Microsoft Active Accessibility использует \_ идентификатор объекта куерикласснамеидкс OBJID с \_ сообщением WM getobject для определения класса, к которому принадлежит стандартный элемент управления Windows или общий элемент управления.
ms.assetid: 2167df6d-5df3-40b7-bebe-142f4bd98cd7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2ba7d73a152380411ef0b230de8f0e3372a6718b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064073"
---
# <a name="the-objid_queryclassnameidx-object-identifier"></a>\_Идентификатор объекта КУЕРИКЛАССНАМЕИДКС OBJID

Microsoft Active Accessibility использует идентификатор [**объекта \_ куерикласснамеидкс OBJID**](object-identifiers.md) с сообщением [**WM \_ getobject**](wm-getobject.md) для определения класса, к которому принадлежит стандартный элемент управления Windows или общий элемент управления. Элемент управления реагирует на это сообщение, возвращая значение, которое Microsoft Active Accessibility сопоставляется с именем класса элемента управления. Microsoft Active Accessibility использует эти сведения, чтобы обеспечить поддержку специальных возможностей для стандартных элементов управления Windows и стандартных элементов управления.

как правило, только стандартные элементы управления Windows и общие элементы управления реагируют на идентификатор объекта [**\_ куерикласснамеидкс OBJID**](object-identifiers.md) . однако пользовательский элемент управления также может отвечать, если он включает все те же функциональные возможности, что и существующий стандартный элемент управления Windows или обычный элемент управления. Это обеспечивает поддержку пользовательского элемента управления одним из стандартных прокси-объектов, предоставляемых Microsoft Active Accessibility.

Дополнительные сведения см. в [приложении F: значения идентификаторов объектов для OBJID \_ куерикласснамеидкс](appendix-f--object-identifier-values-for-objid-queryclassnameidx.md).

 

 




