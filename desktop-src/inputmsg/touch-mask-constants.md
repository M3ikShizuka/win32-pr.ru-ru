---
title: Маска касания
description: Значения, которые могут отображаться в поле Таучмаск структуры POINTER_TOUCH_INFO.
ms.assetid: 23AD50C8-C769-48D6-9F27-DB2755C03D5C
topic_type:
- apiref
api_name:
- TOUCH_MASK_NONE
- TOUCH_MASK_CONTACTAREA
- TOUCH_MASK_ORIENTATION
- TOUCH_MASK_PRESSURE
api_location:
- winuser.h
api_type:
- HeaderDef
ms.topic: article
ms.date: 02/03/2020
ms.openlocfilehash: 3643b30f378e4a6dacae751e9778f57d39a19da9a7fddfdfa48bd2e2acfac464
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120015214"
---
# <a name="touch-mask"></a>Маска касания

Значения, которые могут отображаться в поле **таучмаск** структуры [**POINTER_TOUCH_INFO**](/previous-versions/windows/desktop/api) .

<dl> <dt>

<span id="TOUCH_MASK_NONE_"></span><span id="touch_mask_none_"></span>**TOUCH_MASK_NONE** 
</dt> <dd> <dl> <dt>

0x00000000
</dt> <dt>



По умолчанию. Все необязательные поля являются недопустимыми.


</dt> </dl> </dd> <dt>

<span id="TOUCH_MASK_CONTACTAREA"></span><span id="touch_mask_contactarea"></span>**TOUCH_MASK_CONTACTAREA**
</dt> <dd> <dl> <dt>

0x00000001
</dt> <dt>



**ркконтакт** структуры [**POINTER_TOUCH_INFO**](/previous-versions/windows/desktop/api) является допустимой.


</dt> </dl> </dd> <dt>

<span id="TOUCH_MASK_ORIENTATION"></span><span id="touch_mask_orientation"></span>**TOUCH_MASK_ORIENTATION**
</dt> <dd> <dl> <dt>

0x00000002
</dt> <dt>



допустима **ориентация** структуры [**POINTER_TOUCH_INFO**](/previous-versions/windows/desktop/api) .


</dt> </dl> </dd> <dt>

<span id="TOUCH_MASK_PRESSURE"></span><span id="touch_mask_pressure"></span>**TOUCH_MASK_PRESSURE**
</dt> <dd> <dl> <dt>

0x00000004
</dt> <dt>



неправильное **давление** структуры [**POINTER_TOUCH_INFO**](/previous-versions/windows/desktop/api) .


</dt> </dl> </dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Winuser. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Константы](constants.md)
</dt> <dt>

[**POINTER_INFO**](/previous-versions/windows/desktop/api)
</dt> </dl>

 

 





