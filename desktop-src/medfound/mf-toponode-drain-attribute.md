---
description: Указывает, когда преобразуются преобразования.
ms.assetid: 68332106-d1fe-467b-8baa-1e592b9cc243
title: Атрибут MF_TOPONODE_DRAIN (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 679b87d626738b82f4504673392bd0fe159e2722
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579863"
---
# <a name="mf_toponode_drain-attribute"></a>\_ \_ Атрибут слива MF топоноде

Указывает, когда преобразуются преобразования.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Этот атрибут применяется к узлам преобразования (**\_ \_ \_ узел преобразования топологии MF**).

Значение атрибута является членом перечисления [**\_ \_ \_ режима стока топоноде**](/windows/desktop/api/mfidl/ne-mfidl-mf_toponode_drain_mode) . Если этот атрибут не задан, по умолчанию используется значение **MF \_ топоноде \_ сток \_ по умолчанию**.

Сток выполняется путем вызова [**имфтрансформ::P роцессмессаже**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-processmessage) в преобразовании с сообщением о [**\_ \_ \_ стоке команды сообщения MFT**](mft-message-command-drain.md) . Дополнительные сведения см. в статье перечисление [**\_ \_ типов сообщений MFT**](/windows/desktop/api/mftransform/ne-mftransform-mft_message_type) .

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

 

 




