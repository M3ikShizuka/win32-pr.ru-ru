---
description: Указывает, использует ли источник аппаратного устройства Системное время для меток времени.
ms.assetid: 54cdfa13-955a-4e92-b337-f645d526a1b8
title: Атрибут MFT_HW_TIMESTAMP_WITH_QPC_Attribute (Мфтрансформ. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: af0081c384af4e0fb36da10d87979c1e2d9ad0256f474581f1be3d9fce213cc1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120012654"
---
# <a name="mft_hw_timestamp_with_qpc_attribute-attribute"></a>\_ \_ Метка времени в MFT HW \_ с \_ \_ атрибутом атрибута QPC

Указывает, использует ли источник аппаратного устройства Системное время для меток времени.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес:: UInt32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32).

Чтобы задать этот атрибут, вызовите [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32).

## <a name="remarks"></a>Remarks

Если этот атрибут имеет **значение true**, источник устройства использует системное время, возвращаемое **QueryPerformanceCounter**, для меток времени. В противном случае источник устройства использует часы устройства. Значение по умолчанию — **FALSE**.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для настольных приложений Server 2008 R2 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Мфтрансформ. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Запись атрибутов устройства](capture-device-attributes.md)
</dt> </dl>

 

 




