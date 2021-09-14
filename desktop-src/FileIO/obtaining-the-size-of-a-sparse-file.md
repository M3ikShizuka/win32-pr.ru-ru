---
description: Получите выделенный размер или общий размер файла с помощью функции Жеткомпресседфилесизе или GetFileSize.
ms.assetid: 1894ea01-49ff-41e3-9912-1cd75966bd3f
title: Получение размера разреженного файла
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e93a1c6a33f0d6913e0e6848e4593ea0e0bf0259
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057843"
---
# <a name="obtaining-the-size-of-a-sparse-file"></a>Получение размера разреженного файла

Используйте функцию [**жеткомпресседфилесизе**](/windows/desktop/api/fileapi/nf-fileapi-getcompressedfilesizea) , чтобы получить фактический размер, выделенный на диске для разреженного файла. Этот итог не включает размер регионов, которые были освобождены, так как они заполнены нулями. Используйте функцию [**GetFileSize**](/windows/desktop/api/FileAPI/nf-fileapi-getfilesize) , чтобы определить общий размер файла, включая размер разреженных регионов, которые были освобождены.

 

 



