---
title: Сопоставление интерфейсов ADSI с функциями управления сетью
description: Интерфейсы служб Active Directory (ADSI) представляют собой набор COM-интерфейсов, используемых для доступа к возможностям служб каталогов от разных поставщиков сети.
ms.assetid: dfa81c58-3ce4-40ee-8bfc-a19a13781992
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e5ed9411989d5db754326a7a89130deada129fa6a58322ddef7e118772960d71
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119912053"
---
# <a name="mapping-adsi-interfaces-to-the-network-management-functions"></a>Сопоставление интерфейсов ADSI с функциями управления сетью

Интерфейсы служб Active Directory (ADSI) представляют собой набор COM-интерфейсов, используемых для доступа к возможностям служб каталогов от разных поставщиков сети. ADSI представляет единый набор интерфейсов службы каталогов для управления сетевыми ресурсами в распределенной вычислительной среде.

При программировании для Active Directory вы можете вызывать определенные методы интерфейса ADSI для достижения тех же функций, которые можно достичь, вызывая определенные функции управления сетью.

В следующей таблице перечислены функции управления сетью и группы функций, а также интерфейсы ADSI, к которым сопоставляются функции.



| Функции                                                                  | Интерфейсы                                                                                             |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| [**Нетфилинум**](/windows/desktop/api/lmshare/nf-lmshare-netfileenum), [ **нетфилежетинфо**](/windows/desktop/api/lmshare/nf-lmshare-netfilegetinfo) | [**Иадсресаурце**](/windows/desktop/api/iads/nn-iads-iadsresource), [ **иадсфилесервицеоператионс**](/windows/desktop/api/iads/nn-iads-iadsfileserviceoperations) |
| [Групп](group-functions.md)\*                                          | [**иадсграуп**](/windows/desktop/api/iads/nn-iads-iadsgroup)                                                                        |
| [нетлокалграуп](local-group-functions.md)\*                               | [**иадсграуп**](/windows/desktop/api/iads/nn-iads-iadsgroup)                                                                        |
| [нетсервер](server-functions.md)\*                                        | [**иадскомпутер**](/windows/desktop/api/iads/nn-iads-iadscomputer)                                                                  |
| [нетсессион](session-functions.md)\*                                      | [**Иадссессион**](/windows/desktop/api/iads/nn-iads-iadssession), [ **иадсфилесервицеоператионс**](/windows/desktop/api/iads/nn-iads-iadsfileserviceoperations)   |
| [нетшаре](share-functions.md)\*                                          | [**иадсфилешаре**](/windows/desktop/api/iads/nn-iads-iadsfileshare)                                                                |
| [нетусер](user-functions.md)\*                                            | [**IADsUser**](/windows/desktop/api/iads/nn-iads-iadsuser), [ **иадскомпутер**](/windows/desktop/api/iads/nn-iads-iadscomputer)                                   |
| [нетусермодалс](user-modal-functions.md)\*                                | [**иадсдомаин**](/windows/desktop/api/iads/nn-iads-iadsdomain)                                                                      |



 

Дополнительные сведения о службах каталогов и программировании с помощью ADSI см. в разделе [интерфейсы служб Active Directory](/windows/desktop/ADSI/active-directory-service-interfaces-adsi). Сведения о пользовательских свойствах, которые поставщик WinNT предоставляет для класса User, а также методы свойств интерфейса [**IADsUser**](/windows/desktop/api/iads/nn-iads-iadsuser) , который поставщик WinNT не поддерживает, см. в разделе [поставщик ADSI WinNT](/windows/desktop/ADSI/adsi-winnt-provider).

 

 