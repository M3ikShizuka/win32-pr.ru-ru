---
title: Windows Сетевые операции
description: Приложение может использовать функции Внет для просмотра, добавления или отмены сетевых подключений в любом месте иерархии сети.
ms.assetid: 8f17af6c-e1b2-4b53-b3f0-698d42beb704
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: aa1763f7261dd17fa6f21355ef2f1de404c2b34ec13d6ad6e9769aee3be55283
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119760344"
---
# <a name="windows-networking-operations"></a>Windows Сетевые операции

Приложение может использовать функции Внет для просмотра, добавления или отмены сетевых подключений в любом месте иерархии сети.

*Постоянное подключение* — это сетевое подключение, которое система автоматически восстанавливает при входе пользователя в систему. Вы можете вызвать функции [**WNetAddConnection2**](/windows/win32/api/winnetwk/nf-winnetwk-wnetaddconnection2a) (или [**WNetAddConnection3**](/windows/win32/api/winnetwk/nf-winnetwk-wnetaddconnection3a)) и [**WNetCancelConnection2**](/windows/win32/api/winnetwk/nf-winnetwk-wnetcancelconnection2a) , чтобы управлять тем, является ли сетевое подключение постоянным от одного сеанса к другому.

Чтобы найти имя пользователя по умолчанию или имя пользователя, используемое для установления сетевого подключения, вызовите функцию [**внетжетусер**](/windows/win32/api/winnetwk/nf-winnetwk-wnetgetusera) .

Помимо вызова функций Внет, процесс также может использовать маилслотс и именованные каналы для взаимодействия с другим процессом. Дополнительные сведения см. в разделе [маилслотс](/windows/desktop/ipc/mailslots) и [каналы](/windows/desktop/ipc/pipes).

 

 