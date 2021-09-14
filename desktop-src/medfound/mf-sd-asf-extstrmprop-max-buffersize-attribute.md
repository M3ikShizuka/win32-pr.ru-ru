---
description: Указывает максимальный размер буфера в байтах, необходимый для потока в файле ASF.
ms.assetid: 1704a70a-a52b-4e7d-8a32-d0c4e97f8cc2
title: Атрибут MF_SD_ASF_EXTSTRMPROP_MAX_BUFFERSIZE (Вмконтаинер. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ce31dfacd1d53cadcc38b37e1cb755c330a7882f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127263264"
---
# <a name="mf_sd_asf_extstrmprop_max_buffersize-attribute"></a>MF \_ SD \_ ASF \_ екстстрмпроп \_ Max, \_ атрибут BUFFERSIZE

Указывает максимальный размер буфера в байтах, необходимый для потока в файле ASF.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Этот атрибут применяется к дескрипторам потоков для содержимого ASF. Он соответствует полю "Размер альтернативного буфера" в объекте свойств расширенного потока. Дополнительные сведения см. в спецификации ASF.

Метод [**имфасфконтентинфо:: женератепресентатиондескриптор**](/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfcontentinfo-generatepresentationdescriptor) создает этот атрибут из метаданных ASF. Приложение может создать дескриптор потока для потока из дескриптора представления путем вызова [**имфпресентатиондескриптор:: жетстреамдескрипторбиндекс**](/windows/desktop/api/mfidl/nf-mfidl-imfpresentationdescriptor-getstreamdescriptorbyindex).

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

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[**имфстреамдескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfstreamdescriptor)
</dt> <dt>

[Атрибуты дескриптора потока](stream-descriptor-attributes.md)
</dt> <dt>

[Объект заголовка ASF](asf-file-structure.md)
</dt> </dl>

 

 




