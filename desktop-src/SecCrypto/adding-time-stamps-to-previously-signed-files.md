---
description: Метки времени обычно включаются, когда файл подписывается с помощью средства SignTool с параметром-t.
ms.assetid: ca22d055-dc34-447c-991b-27ff21ca3afc
title: Добавление меток времени в ранее подписанные файлы
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ef2e750dcb178b2a089bfbde0b2aea882b097c86
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173315"
---
# <a name="adding-time-stamps-to-previously-signed-files"></a>Добавление меток времени в ранее подписанные файлы

Метки времени обычно включаются, когда файл подписывается с помощью средства SignTool с параметром **-t** . Кроме того, метки времени можно добавлять к файлам, которые были подписаны без отметки времени. Следующая команда добавляет отметку времени к ранее подписанному файлу:

**Метка времени SignTool-t HTTPS: \/ /timestamp.digicert.com *MyControl.exe***

> [!Note]  
> Файл, к которому отметок времени, должен быть ранее подписан.

 

Дополнительные сведения о SignTool см. в разделе [SignTool](signtool.md).

 

 



