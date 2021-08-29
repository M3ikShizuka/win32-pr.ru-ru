---
description: Приложение может программно создавать и удалять каталоги.
ms.assetid: 52d1d8a8-e5a7-44f5-9bf2-2a496ef79d32
title: Создание и удаление каталогов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 862907ad3adef3a4502961820a6f5ffcb1cd932541b03226854d81372ca6e13f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119533743"
---
# <a name="creating-and-deleting-directories"></a>Создание и удаление каталогов

Приложение может программно создавать и удалять каталоги.

Чтобы создать новый каталог, используйте функцию [**CreateDirectory**](/windows/desktop/api/FileAPI/nf-fileapi-createdirectorya), [**креатедиректорекс**](/windows/desktop/api/WinBase/nf-winbase-createdirectoryexa)или [**креатедиректоритрансактед**](/windows/desktop/api/WinBase/nf-winbase-createdirectorytransacteda) . Каталогу присваивается имя, указанное при его создании. Соглашения об именовании каталога следуют правилам именования файлов. Описание этих соглашений см. [в разделе Присвоение имени файлу](naming-a-file.md).

Чтобы удалить существующий каталог, используйте функцию [**ремоведиректори**](/windows/desktop/api/FileAPI/nf-fileapi-removedirectorya) или [**ремоведиректоритрансактед**](/windows/desktop/api/WinBase/nf-winbase-removedirectorytransacteda) . Перед удалением каталога необходимо убедиться, что каталог пуст и у вас есть права на удаление для каталога. Чтобы выполнить Последнее действие, вызовите функцию [**жетсекуритинфо**](/windows/desktop/api/aclapi/nf-aclapi-getsecurityinfo) .

 

 
