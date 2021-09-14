---
description: Свойство UpgradeCode представляет собой идентификатор GUID, представляющий связанный набор продуктов. Значение UpgradeCode используется в таблице Upgrade для поиска связанных версий уже установленных продуктов. Это свойство используется действием Регистерпродукт.
ms.assetid: 6cdee5d8-8aa0-4fad-9338-152ee33b8077
title: UpgradeCode, свойство
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ac1e5493ad651e609f6ef9d7ae14e07c0c15b5b4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254104"
---
# <a name="upgradecode-property"></a>UpgradeCode, свойство

Свойство **UpgradeCode** представляет собой идентификатор GUID, представляющий связанный набор продуктов. Значение **UpgradeCode** используется в [таблице Upgrade](upgrade-table.md) для поиска связанных версий уже установленных продуктов.

Это свойство используется [действием регистерпродукт](registerproduct-action.md).

## <a name="remarks"></a>Remarks

Настоятельно рекомендуется, чтобы авторы установочных пакетов указали **UpgradeCode** для своего приложения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP. сведения о минимальном Windows пакета обновления, который требуется для установщик Windows версии, см. в [установщик Windows требования к Run-Time](windows-installer-portal.md) .<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Свойства](properties.md)
</dt> <dt>

[Установка исправлений и обновления](patching-and-upgrades.md)
</dt> <dt>

[Подготовка приложения к будущим основным обновлениям](preparing-an-application-for-future-major-upgrades.md)
</dt> </dl>

 

 




