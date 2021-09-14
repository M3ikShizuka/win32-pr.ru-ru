---
description: Содержит секретные данные для зашифрованного файла расширенных систем (ASF). Этот атрибут соответствует полю данных секрета в заголовке шифрования содержимого, определенном в спецификации ASF.
ms.assetid: e6ce71d6-59cd-42da-906a-ab71f2bef16f
title: Атрибут MF_PD_ASF_CONTENTENCRYPTION_SECRET_DATA (Вмконтаинер. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 28c960131e61e539fa417e1068b45974a24c42a3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257824"
---
# <a name="mf_pd_asf_contentencryption_secret_data-attribute"></a>\_ \_ \_ \_ Атрибут данных секрета MF PD ASF контентенкриптион \_

Содержит секретные данные для зашифрованного файла расширенных систем (ASF). Этот атрибут соответствует полю данных секрета в заголовке шифрования содержимого, определенном в спецификации ASF.

## <a name="data-type"></a>Тип данных

массив байтов;

## <a name="remarks"></a>Комментарии

Этот атрибут применяется к дескрипторам представления для содержимого ASF.

Метод [**имфасфконтентинфо:: женератепресентатиондескриптор**](/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfcontentinfo-generatepresentationdescriptor) заполняет массив байтов полем секретных данных. Размер массива равен значению поля "Секретная длина данных" заголовка шифрования содержимого.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Вмконтаинер. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: BLOB**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getblob)
</dt> <dt>

[**Имфаттрибутес:: SetBlob**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setblob)
</dt> <dt>

[**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor)
</dt> <dt>

[Атрибуты дескриптора представления](presentation-descriptor-attributes.md)
</dt> <dt>

[Объект заголовка ASF](asf-file-structure.md)
</dt> <dt>

[Дескрипторы представления](presentation-descriptors.md)
</dt> </dl>

 

 




