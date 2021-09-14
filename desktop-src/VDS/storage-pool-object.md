---
description: Объект пула носителей моделирует пул носителей в подсистеме хранения.
ms.assetid: a6104742-3ef9-4570-9728-3e6580953117
title: служба хранилища Объект Pool
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8c44719b825193faa75546ba1a0f7b42155a3e49
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126890373"
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



 

 

 
