---
description: Векторные обработчики исключений являются расширением для структурированной обработки исключений.
ms.assetid: e4cf8a88-1bdf-4666-8653-fe2e86c4d8ef
title: Обработка векторных исключений
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 011310b46ce8912e03b6481e9b12b986174a3ef0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127164544"
---
# <a name="vectored-exception-handling"></a>Обработка векторных исключений

Векторные обработчики исключений являются расширением для структурированной обработки исключений. Приложение может зарегистрировать функцию для просмотра или обработки всех исключений приложения. Векторные обработчики не основаны на кадрах, поэтому можно добавить обработчик, который будет вызываться независимо от того, где находится в кадре вызова. Векторные обработчики вызываются в том порядке, в котором они были добавлены, когда отладчик получает первое уведомление о шансе, но до того, как система начнет раскрутить стек.

Чтобы добавить векторный обработчик Continue, используйте функцию [**аддвекторедконтинуехандлер**](/windows/win32/api/errhandlingapi/nf-errhandlingapi-addvectoredcontinuehandler) . Чтобы удалить этот обработчик, используйте функцию [**ремовевекторедконтинуехандлер**](/windows/win32/api/errhandlingapi/nf-errhandlingapi-removevectoredcontinuehandler) .

Чтобы добавить векторный обработчик исключений, используйте функцию [**аддвекторедексцептионхандлер**](/windows/win32/api/errhandlingapi/nf-errhandlingapi-addvectoredexceptionhandler) . Чтобы удалить этот обработчик, используйте функцию [**ремовевекторедексцептионхандлер**](/windows/win32/api/errhandlingapi/nf-errhandlingapi-removevectoredexceptionhandler) .

 

 
