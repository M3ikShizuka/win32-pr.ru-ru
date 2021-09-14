---
description: KTM определяет следующие маски доступа прикрепления, которые будут использоваться при открытии зачислений.
ms.assetid: 93773eb7-141a-49f3-9306-ffbda2f4ab9f
title: Маски доступа прикрепления (WinNT. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 63e4ebd67f93368215ebcdcd362595d0341adb52
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144766"
---
# <a name="enlistment-access-masks"></a>Маски доступа прикрепления

KTM определяет следующие маски доступа прикрепления, которые будут использоваться при открытии зачислений.

<dl> <dt>

<span id="ENLISTMENT_QUERY_INFORMATION"></span><span id="enlistment_query_information"></span>**\_сведения о запросе ПРИкрепления \_**
</dt> <dd> <dl> <dt>

Номера 0x00001
</dt> <dt>



Вызывающий объект может запросить в KTM сведения о зачислении.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_SET_INFORMATION"></span><span id="enlistment_set_information"></span>**\_сведения о наборе ЗАчислений \_**
</dt> <dd> <dl> <dt>

0x00002
</dt> <dt>



Вызывающий объект может задавать сведения о зачислении.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_RECOVER"></span><span id="enlistment_recover"></span>**Восстановление прикрепления \_**
</dt> <dd> <dl> <dt>

0x00004
</dt> <dt>



Вызывающий объект может восстановить зачисление.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_SUBORDINATE_RIGHTS"></span><span id="enlistment_subordinate_rights"></span>**\_подчиненные права ПРИкрепления \_**
</dt> <dd> <dl> <dt>

0x00008
</dt> <dt>



Вызывающий объект может выполнять действия, выполняемые диспетчером ресурсов от имени транзакции. Ниже приведен список действий.

-   [**коммиткомплете**](/windows/desktop/api/Ktmw32/nf-ktmw32-commitcomplete)
-   [**препарекомплете**](/windows/desktop/api/Ktmw32/nf-ktmw32-preparecomplete)
-   [**препрепарекомплете**](/windows/desktop/api/Ktmw32/nf-ktmw32-prepreparecomplete)
-   [**роллбакккомплете**](/windows/desktop/api/Ktmw32/nf-ktmw32-rollbackcomplete)
-   [**реадонленлистмент**](/windows/desktop/api/Ktmw32/nf-ktmw32-readonlyenlistment)
-   [**роллбаккенлистмент**](/windows/desktop/api/Ktmw32/nf-ktmw32-rollbackenlistment)
-   [**синглефасережект**](/windows/desktop/api/Ktmw32/nf-ktmw32-singlephasereject)


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_SUPERIOR_RIGHTS"></span><span id="enlistment_superior_rights"></span>**\_старшие права ПРИкрепления \_**
</dt> <dd> <dl> <dt>

0x00010
</dt> <dt>



Вызывающий объект может быть прикреплен в транзакции в качестве старшего диспетчера транзакций.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_GENERIC_READ"></span><span id="enlistment_generic_read"></span>**\_универсальное чтение ПРИкрепления \_**
</dt> <dd> <dl> <dt>

0x20001
</dt> <dt>



Вызывающий объект имеет следующие привилегии: **стандартные \_ права на \_ Чтение** и **Прикрепление \_ \_**.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_GENERIC_WRITE"></span><span id="enlistment_generic_write"></span>**\_Универсальная запись ПРИкрепления \_**
</dt> <dd> <dl> <dt>

0x2001E
</dt> <dt>



Вызывающий объект имеет следующие привилегии: **стандартные \_ права на \_ запись**, **\_ \_ сведения о наборе зачислений** и **Прикрепление к \_ восстановлению**.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_GENERIC_EXECUTE"></span><span id="enlistment_generic_execute"></span>**\_универсальное выполнение ПРИкрепления \_**
</dt> <dd> <dl> <dt>

0x2001C
</dt> <dt>



Вызывающий объект имеет следующие привилегии **: \_ \_ выполнение стандартных прав**, **\_ Восстановление прикрепления** и **\_ подчиненные \_ права прикрепления**.


</dt> </dl> </dd> <dt>

<span id="ENLISTMENT_ALL_ACCESS"></span><span id="enlistment_all_access"></span>**\_доступ ко всем операциям ПРИкрепления \_**
</dt> <dd> <dl> <dt>

0xF001F
</dt> <dt>



Это значение задает все допустимые биты для значения доступа к зачислению.


</dt> </dl> </dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Файл WinNT. h</dt> </dl> |



 

 




