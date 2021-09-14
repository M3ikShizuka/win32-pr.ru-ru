---
title: Использование асинхронного RPC с каналами DCE
description: Microsoft RPC поддерживает использование каналов DCE. Несмотря на то, что они имеют одинаковое имя, каналы DCE не связаны с именованными каналами. Именованные каналы являются транспортным протоколом. Каналы DCE — это не зависящий от протокола метод обмена данными между клиентом и сервером.
ms.assetid: 9de4f6dc-0aa9-446e-b68c-e0d1e247fea7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 43e9c98f4d4191a064d78cff2c918077f27d676f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064831"
---
# <a name="using-asynchronous-rpc-with-dce-pipes"></a>Использование асинхронного RPC с каналами DCE

Microsoft RPC поддерживает использование каналов DCE. Несмотря на то, что они имеют одинаковое имя, каналы DCE не связаны с [именованными каналами](asynchronous-rpc-over-the-named-pipe-protocol.md). Именованные каналы являются транспортным протоколом. Каналы DCE — это не зависящий от протокола метод обмена данными между клиентом и сервером.

В этом разделе представлено обсуждение RPC с использованием асинхронных каналов DCE. Он разделен на следующие разделы:

-   [Асинхронные каналы](asynchronous-pipes.md)
-   [Объявление асинхронных каналов](declaring-asynchronous-pipes.md)
-   [Асинхронная обработка канала на стороне клиента](client-side-asynchronous-pipe-handling.md)
-   [Обработка асинхронных каналов на стороне сервера](server-side-asynchronous-pipe-handling.md)

Пример приложения RPC с асинхронным каналом см. в образце Филереп в пакете SDK для платформы.

 

 




