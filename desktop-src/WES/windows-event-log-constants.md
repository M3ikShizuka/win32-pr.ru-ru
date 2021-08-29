---
title: Windows Константы журнала событий (Виневт. h)
description: Windows В журнале событий определены следующие константы.
ms.assetid: d3a4a136-ca33-4dad-95ad-af1be6687843
topic_type:
- apiref
api_name:
- EVT_VARIANT_TYPE_MASK
- EVT_VARIANT_TYPE_ARRAY
- EVT_READ_ACCESS
- EVT_WRITE_ACCESS
- EVT_CLEAR_ACCESS
- EVT_ALL_ACCESS
api_location:
- WinEvt.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a7fe5ecd134749e3420b43c621e506930ede982a271652083086175cea1549ea
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119620164"
---
# <a name="windows-event-log-constants"></a>Windows Константы журнала событий

Windows В журнале событий определены следующие константы.

<dl> <dt>

<span id="EVT_VARIANT_TYPE_MASK"></span><span id="evt_variant_type_mask"></span>**\_ \_ маска типа варианта \_ evt**
</dt> <dd> <dl> <dt>

0x7F
</dt> <dt>



Битовая маска, используемая для маскирования бита массива типа Variant, чтобы можно было определить тип данных значения типа Variant, содержащегося в структуре [**evt \_ Variant**](/windows/desktop/api/WinEvt/ns-winevt-evt_variant) .


</dt> </dl> </dd> <dt>

<span id="EVT_VARIANT_TYPE_ARRAY"></span><span id="evt_variant_type_array"></span>**\_массив вариативных \_ типов \_ Variant**
</dt> <dd> <dl> <dt>

128
</dt> <dt>



Этот бит устанавливается для элемента **типа** в структуре параметра [**evt \_**](/windows/desktop/api/WinEvt/ns-winevt-evt_variant) , если вариант содержит указатель на массив значений, а не само значение.


</dt> </dl> </dd> <dt>

<span id="EVT_READ_ACCESS"></span><span id="evt_read_access"></span>**проevt \_ доступ на чтение \_**
</dt> <dd> <dl> <dt>

0x1
</dt> <dt>



Разрешение на управление доступом на чтение, позволяющее считывать данные из журнала событий.


</dt> </dl> </dd> <dt>

<span id="EVT_WRITE_ACCESS"></span><span id="evt_write_access"></span>**\_доступ на запись для ПРОevt \_**
</dt> <dd> <dl> <dt>

0x2
</dt> <dt>



Разрешение на запись контроля доступа, позволяющее записывать данные в журнал событий.


</dt> </dl> </dd> <dt>

<span id="EVT_CLEAR_ACCESS"></span><span id="evt_clear_access"></span>**\_четкий \_ доступ к evt**
</dt> <dd> <dl> <dt>

0x4
</dt> <dt>



Очистите разрешение на контроль доступа, позволяющее очищать всю информацию из журнала событий.


</dt> </dl> </dd> <dt>

<span id="EVT_ALL_ACCESS"></span><span id="evt_all_access"></span>**проevt \_ весь \_ доступ**
</dt> <dd> <dl> <dt>

0x7
</dt> <dt>



Все разрешения на управление доступом (чтение, запись, очистка и удаление).


</dt> </dl> </dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                      |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Виневт. h</dt> </dl> |



 

 





