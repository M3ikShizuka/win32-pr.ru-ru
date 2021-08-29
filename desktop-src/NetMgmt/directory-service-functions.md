---
title: Функции службы каталогов (Управление сетью)
description: Функции службы каталогов управления сетью позволяют разработчикам работать с контроллером домена и членством в домене в службе каталогов.
ms.assetid: 9eeb8f40-85c0-49db-a307-193703e4f463
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3e3f650ab3101cb26c90ae4d6f3854ed2b84ef4ab8c83ed37172eaf7f0c51fa6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119912294"
---
# <a name="directory-service-functions"></a>Функции службы каталогов

Функции службы каталогов управления сетью позволяют разработчикам работать с контроллером домена и членством в домене в службе каталогов.

Функции службы каталогов управления сетью перечислены ниже.



| Функция                                                                 | Описание                                                                                                                                                                                 |
|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**нетаддалтернатекомпутернаме**](/windows/desktop/api/Lmjoin/nf-lmjoin-netaddalternatecomputername)       | Добавляет альтернативное имя для указанного компьютера.                                                                                                                                          |
| [**нетенумератекомпутернамес**](/windows/desktop/api/Lmjoin/nf-lmjoin-netenumeratecomputernames)           | Перечисляет имена для указанного компьютера.                                                                                                                                                |
| [**нетжетжоинаблеаус**](/windows/desktop/api/Lmjoin/nf-lmjoin-netgetjoinableous)                           | Извлекает список подразделений (OU), в которых может быть создана учетная запись компьютера.                                                                                                  |
| [**нетжетжоининформатион**](/windows/desktop/api/Lmjoin/nf-lmjoin-netgetjoininformation)                   | Возвращает сведения о состоянии присоединение для указанного компьютера.                                                                                                                               |
| [**нетжоиндомаин**](/windows/desktop/api/Lmjoin/nf-lmjoin-netjoindomain)                                   | Присоединяет компьютер к Рабочей группе или домену.                                                                                                                                                  |
| [**нетпровисионкомпутераккаунт**](/windows/desktop/api/Lmjoin/nf-lmjoin-netprovisioncomputeraccount)       | Подготавливает учетную запись компьютера для последующего использования в операции присоединение к автономному домену.                                                                                                           |
| [**нетремовеалтернатекомпутернаме**](/windows/desktop/api/Lmjoin/nf-lmjoin-netremovealternatecomputername) | Удаляет альтернативное имя указанного компьютера.                                                                                                                                       |
| [**нетренамемачинеиндомаин**](/windows/desktop/api/Lmjoin/nf-lmjoin-netrenamemachineindomain)             | Изменяет имя компьютера в домене.                                                                                                                                                 |
| [**нетсетпримарикомпутернаме**](/windows/desktop/api/Lmjoin/nf-lmjoin-netsetprimarycomputername)           | Задает имя основного компьютера для указанного компьютера.                                                                                                                                  |
| [**нетунжоиндомаин**](/windows/desktop/api/Lmjoin/nf-lmjoin-netunjoindomain)                               | Отсоединение компьютера от рабочей группы или домена.                                                                                                                                            |
| [**нетвалидатенаме**](/windows/desktop/api/Lmjoin/nf-lmjoin-netvalidatename)                               | Проверка допустимости имени компьютера, имени Рабочей группы или имени домена.                                                                                                                   |



 

Дополнительные сведения о программировании для Active Directory см. в [справочнике по Active Directory](/windows/desktop/AD/active-directory-domain-services-reference). Дополнительные сведения о подразделениях см. в разделе [Управление пользователями](/windows/desktop/AD/managing-users) в документации по Active Directory.

 

 