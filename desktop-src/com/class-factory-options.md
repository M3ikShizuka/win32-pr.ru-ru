---
title: Параметры фабрики класса
description: Параметры фабрики класса
ms.assetid: e9e33e07-7628-4c5e-965d-e12a9c1d69c2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5fab52ea11a0e7e20d10757eb8d6e86577afc35c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574106"
---
# <a name="class-factory-options"></a>Параметры фабрики класса

элемент управления ActiveX, в силу того, что является COM-объектом, должен иметь связанный серверный код, поддерживающий создание элементов управления через [**IClassFactory**](/windows/win32/api/unknwn/nn-unknwn-iclassfactory) как минимум.

Это необязательно, а не обязательно, что этот объект класса также поддерживает [**IClassFactory2**](/windows/desktop/api/OCIdl/nn-ocidl-iclassfactory2) для управления лицензированием. Только те поставщики, которые интересуются лицензией, должны поддерживать механизм лицензирования COM. Иными словами, поскольку **IClassFactory2** является единственным способом обеспечения лицензирования на уровне com, этот интерфейс необходим для объекта класса для тех элементов управления, которые должны быть лицензированы.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Элементы управления](controls.md)
</dt> </dl>

 

 