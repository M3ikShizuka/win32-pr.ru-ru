---
description: поскольку сокеты не представлены в виде неотрицательного целого числа типа UNIX, реализация функции select была изменена в сокетах Windows.
ms.assetid: 97c7996c-c541-4673-b26f-d66f3fc0b62e
title: Макросы SELECT, FD_SET и FD_XXX
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4b9bce15e921bf6566717a30114af73530406e5e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056215"
---
# <a name="select-fd_set-and-fd_xxx-macros"></a>Макросы SELECT, ДЕМОна \_ Set и демона \_ xxx

поскольку сокеты не представлены в виде неотрицательного целого числа типа UNIX, реализация функции [**select**](/windows/desktop/api/Winsock2/nf-winsock2-select) была изменена в сокетах Windows. Каждый набор сокетов по-прежнему представлен структурой **\_ набора** элементов, но вместо сохранения в виде битовой маски набор реализуется как массив сокетов. Чтобы избежать потенциальных проблем, приложения должны придерживаться использования макросов ДЕМОна \_ xxx для установки, инициализации, очистки и проверки структур наборов элементов [**фильтра \_**](/windows/desktop/api/winsock/nf-winsock-fd_set) .

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Перенос приложений сокета в Winsock](porting-socket-applications-to-winsock.md)
</dt> <dt>

[Вопросы программирования Winsock](winsock-programming-considerations.md)
</dt> </dl>

 

 



