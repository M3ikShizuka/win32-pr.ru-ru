---
description: Указывает, как загрузчик топологии подключает этот узел топологии и является ли этот узел необязательным.
ms.assetid: 8d70e1af-607b-47c3-9808-091c95fd05b7
title: Атрибут MF_TOPONODE_CONNECT_METHOD (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e3db5fef529ef451fa02ac4a29e62002b0a1996a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127363912"
---
# <a name="mf_toponode_connect_method-attribute"></a>\_ \_ Атрибут метода Connect топоноде MF \_

Указывает, как загрузчик топологии подключает этот узел топологии и является ли этот узел необязательным.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Этот атрибут применяется ко всем типам узлов.

Значение атрибута представляет собой побитовое **или** для флагов из перечисления [**\_ \_ метода MF Connect**](/windows/desktop/api/mfidl/ne-mfidl-mf_connect_method) . Если этот атрибут не задан, по умолчанию используется значение **MF \_ Connect \_ Разрешить \_ декодер**.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[**имфтопологиноде**](/windows/desktop/api/mfidl/nn-mfidl-imftopologynode)
</dt> <dt>

[Атрибуты узла топологии](topology-node-attributes.md)
</dt> </dl>

 

 




