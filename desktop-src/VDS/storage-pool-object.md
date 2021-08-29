---
description: Объект пула носителей моделирует пул носителей в подсистеме хранения.
ms.assetid: a6104742-3ef9-4570-9728-3e6580953117
title: служба хранилища Объект Pool
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6ee6ddd225c3c6e92f29bc4b4f338d9c3ef7ffc0cf0cc5e748d4bc71da319d19
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119986734"
---
# <a name="storage-pool-object"></a>служба хранилища Объект Pool

\[начиная с Windows 8 и Windows Server 2012, интерфейс COM [службы виртуальных дисков](virtual-disk-service-portal.md) заменяется [API Windows служба хранилища управления](/previous-versions/windows/desktop/stormgmt/windows-storage-management-api-portal).\]

Объект пула носителей моделирует пул носителей в подсистеме хранения.

Пул носителей содержит экстенты дисков с одного или нескольких дисков, управляемых одним и тем же поставщиком оборудования.

В следующей таблице перечислены связанные интерфейсы, перечисления и структуры.



| Тип                                              | Элемент                                                                                                                                                                                                                                                                                                  |
|---------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Интерфейсы, которые всегда предоставляются этим объектом | [**ивдссторажепул**](/windows/desktop/api/Vds/nn-vds-ivdsstoragepool)                                                                                                                                                                                                                                                               |
| Связанные перечисления                           | Служба [**VDS \_ \_Тип RAID**](/windows/desktop/api/Vds/ne-vds-vds_raid_type), [**\_ \_ \_ Состояние пула хранилища VDS**](/windows/desktop/api/Vds/ne-vds-vds_storage_pool_status)и [**\_ \_ \_ Тип пула хранилища VDS**](/windows/desktop/api/Vds/ne-vds-vds_storage_pool_type).                                                                                                                                  |
| Связанные структуры                             | Служба [**VDS \_ HINTS2**](/windows/desktop/api/Vds/ns-vds-vds_hints2), [**\_ \_ Атрибуты пула VDS**](/windows/desktop/api/Vds/ns-vds-vds_pool_attributes), [**\_ \_ настраиваемые \_ Атрибуты пула службы VDS**](/windows/desktop/api/Vds/ns-vds-vds_pool_custom_attributes), [**\_ \_ \_ \_ область диска пула носителей VDS**](/windows/desktop/api/Vds/ns-vds-vds_storage_pool_drive_extent)и " [**\_ \_ \_ prop" пула носителей VDS**](/windows/desktop/api/Vds/ns-vds-vds_storage_pool_prop). |



 

 

 
