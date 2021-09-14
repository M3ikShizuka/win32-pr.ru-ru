---
description: Классы RealTimeStylus, GestureRecognizer и DynamicRenderer реализуются как оболочки COM и доступны только в управляемом коде.
ms.assetid: db8f0f25-3650-4843-92e4-af5460841e7e
title: Примечания по реализации для API-интерфейсов Стилусинпут
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 47150d6a9aff5495e89f30d29929fd7d604f9eed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247792"
---
# <a name="implementation-notes-for-the-stylusinput-apis"></a>Примечания по реализации для API-интерфейсов Стилусинпут

Классы [**RealTimeStylus**](realtimestylus-class.md), [GestureRecognizer](/previous-versions/ms575185(v=vs.100))и [DynamicRenderer](/previous-versions/ms575176(v=vs.100)) реализуются как оболочки COM и доступны только в управляемом коде.

Когда объект [**RealTimeStylus**](realtimestylus-class.md), [GestureRecognizer](/previous-versions/ms575185(v=vs.100))или [DynamicRenderer](/previous-versions/ms575176(v=vs.100)) добавляется как подключаемый модуль в объект **RealTimeStylus** , базовые COM-объекты взаимодействуют на уровне com. Поэтому непосредственное обращение к методам интерфейсов [истилуссинкплугин](/previous-versions/ms575201(v=vs.100)) или [истилусасинкплугин](/previous-versions/ms575194(v=vs.100)) не поддерживается. Добавление объекта **RealTimeStylus**, GestureRecognizer или DynamicRenderer в объект **RealTimeStylus** является единственным способом доступа к этим функциям.

 

 
