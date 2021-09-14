---
title: Реализация собственного Active Accessibility
description: Говорят, что элементы пользовательского интерфейса, реализующие интерфейс IAccessible, предоставляют собственную реализацию.
ms.assetid: 36a5c0cd-53f0-433e-8932-da7d1de177dd
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b5f6e6b6152c2f5e5c41a6a2b7cd3f84a3fce373
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064139"
---
# <a name="native-active-accessibility-implementation"></a>Реализация собственного Active Accessibility

Говорят, что элементы пользовательского интерфейса, реализующие интерфейс [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) , предоставляют *собственную реализацию*. Несмотря на то, что затраты на разработку для реализации **IAccessible** (или любого другого интерфейса COM) могут быть высокими, преимущество является исчерпывающим элементом управления информацией, предоставляемой клиентам.

Если приложение использует настраиваемые элементы управления или другие элементы управления, которые не могут быть переданы с помощью Oleacc.dll, необходимо предоставить собственную реализацию.

 

 




