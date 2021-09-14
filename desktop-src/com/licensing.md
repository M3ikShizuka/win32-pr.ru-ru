---
title: Лицензирование
description: Лицензирование
ms.assetid: a77c0141-62b4-4032-a734-5a55da6a50e0
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 06066365d2cf00a7b5db6d6ca755261e5a9470fa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127249307"
---
# <a name="licensing"></a>Лицензирование

для успешного внедрения лицензированных элементов управления ActiveX контейнеры элементов управления должны использовать [**IClassFactory2**](/windows/desktop/api/OCIdl/nn-ocidl-iclassfactory2) вместо [**IClassFactory**](/windows/win32/api/unknwn/nn-unknwn-iclassfactory). некоторые вспомогательные функции создания и загрузки OLE ([**олелоад**](/windows/desktop/api/Ole2/nf-ole2-oleload) и [**cocreateinstance**](/windows/desktop/api/combaseapi/nf-combaseapi-cocreateinstance)) явно вызывают **IClassFactory** , а не **IClassFactory2**, и поэтому не могут использоваться для создания или загрузки лицензированных ActiveX элементов управления. контейнеры элементов управления ActiveX должны явно создавать и загружать ActiveX элементы управления с помощью **IClassFactory2**.

 

 