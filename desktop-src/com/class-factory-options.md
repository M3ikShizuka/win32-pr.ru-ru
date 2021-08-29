---
title: Параметры фабрики класса
description: Параметры фабрики класса
ms.assetid: e9e33e07-7628-4c5e-965d-e12a9c1d69c2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 720016aa42057047fa0980c1219dd4fe787198fea4c0ccc7d7f86d45a634a672
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119859584"
---
# <a name="class-factory-options"></a>Параметры фабрики класса

элемент управления ActiveX, в силу того, что является COM-объектом, должен иметь связанный серверный код, поддерживающий создание элементов управления через [**IClassFactory**](/windows/win32/api/unknwn/nn-unknwn-iclassfactory) как минимум.

Это необязательно, а не обязательно, что этот объект класса также поддерживает [**IClassFactory2**](/windows/desktop/api/OCIdl/nn-ocidl-iclassfactory2) для управления лицензированием. Только те поставщики, которые интересуются лицензией, должны поддерживать механизм лицензирования COM. Иными словами, поскольку **IClassFactory2** является единственным способом обеспечения лицензирования на уровне com, этот интерфейс необходим для объекта класса для тех элементов управления, которые должны быть лицензированы.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Элементы управления](controls.md)
</dt> </dl>

 

 