---
title: Модели Memory-Management
description: Модели Memory-Management
ms.assetid: 1690901b-2a1e-455b-a440-2674f5e5dfa4
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b8114f11755829be9d5f7b17b751e075701ac0aa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127244465"
---
# <a name="memory-management-models"></a>Модели Memory-Management

Как разработчик, у вас есть несколько вариантов выделения и освобождения памяти. Рассмотрим сложную структуру данных, состоящую из узлов, связанных с указателями, таких как связанный список или дерево. Можно применять атрибуты, которые выбирают одну из следующих моделей:

-   [Выделение и освобождение узлов по](node-by-node-allocation-and-deallocation.md)узлам.
-   [Один линейный буфер, выделенный заглушкой для всего дерева](stub-allocated-buffers.md).
-   [Управление памятью заглушки сервера](server-stub-memory-management.md)
-   [Один линейный буфер, выделенный клиентским приложением для всего дерева](application-allocated-buffer.md).
-   [Постоянное хранилище на сервере](persistent-storage-on-the-server.md).

 

 




