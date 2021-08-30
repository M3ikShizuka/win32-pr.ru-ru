---
description: Объект Merge предоставляет доступ к другим объектам верхнего уровня. Перед загрузкой поддержки автоматизации, необходимой COM для доступа к функциям в Mergemod.dll, необходимо создать объект слияния.
ms.assetid: 3f76ee8a-d195-4a69-99a3-31ef2c1c72d5
title: Объект Merge
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0d8382fd3c0b94e3e450d56a62fdd9d0a330cdd37fad72a6da926581b6336bc7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119869254"
---
# <a name="merge-object"></a>Объект Merge

Объект **Merge** предоставляет доступ к другим объектам верхнего уровня. Перед загрузкой поддержки автоматизации, необходимой COM для доступа к функциям в Mergemod.dll, необходимо создать объект **слияния** .

Mergemod.dll предоставляет доступ к расширенным функциям во время сборки с помощью второй версии существующего идентификатора CLSID. Этот CLSID поддерживает существующие функции, доступные через интерфейс [**имсммерже**](/windows/win32/api/mergemod/nn-mergemod-imsmmerge) , но интерфейс по умолчанию для объекта (и связанный с ним сдвоенный интерфейс) является интерфейсом [**IMsmMerge2**](/windows/desktop/api/Mergemod/nn-mergemod-imsmmerge2) , а не интерфейсом **имсммерже** .

 

 
