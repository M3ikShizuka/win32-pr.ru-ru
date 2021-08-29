---
description: Чтобы добавить элемент в подменю программы, выполните следующие действия.
ms.assetid: F8793C33-2281-4E4A-9659-4189E1C8279A
title: Добавление ярлыков в меню "Пуск"
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4b8c31f8180f4bd0d3b8aa8252d7c3f1fedc4238bb5320f8179f3a4fd4b497b1
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118969433"
---
# <a name="how-to-add-shortcuts-to-the-start-menu"></a>Добавление ярлыков в меню "Пуск"

Чтобы добавить элемент в подменю **программы** , выполните следующие действия.

## <a name="instructions"></a>Инструкции

### <a name="step-1"></a>Шаг 1.

Создайте [ссылку на оболочку](./links.md) с помощью интерфейса [**ишелллинк**](/windows/desktop/api/Shobjidl_core/nn-shobjidl_core-ishelllinka) .

### <a name="step-2"></a>Шаг 2.

Получите расположение папки Programs с помощью функции [**шжеткновнфолдерпас**](/windows/desktop/api/shlobj_core/nf-shlobj_core-shgetknownfolderpath) , передав [**\_ программы FOLDERID**](knownfolderid.md).

### <a name="step-3"></a>Шаг 3.

Добавьте ссылку оболочки в папку программы. Можно также создать папку в папке Programs и добавить ссылку в эту папку.

 

 
