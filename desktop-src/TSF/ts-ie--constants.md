---
title: Константы TS_IE_ (Текстстор. h)
description: '\_Константы служб терминалов IE \_ \ описывают, как вставить текст, который может содержать внедренные объекты, используемые текстовыми службами.'
ms.assetid: a455d712-42d5-472e-862d-85ae3ba9149f
topic_type:
- apiref
api_name:
- TS_IE_CORRECTION
- TS_IE_COMPOSITION
api_location:
- Textstor.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d9abdb05ba065ed9bf41b5379060c0643053884e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056743"
---
# <a name="ts_ie_-constants"></a>\_Константы служб терминалов IE \_ \*

\_Константы служб терминалов IE \_ \* описывают, как вставить текст, который может содержать внедренные объекты, используемые текстовыми службами.



| Константа/значение                                                                                                                                                                                                                          | Описание                                                                                                                                                                           |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="TS_IE_CORRECTION"></span><span id="ts_ie_correction"></span><dl> <dt>**TS \_ \_Исправление IE**</dt> <dt>(0x1)</dt> </dl>    | Текст представляет собой преобразование (исправление) существующего содержимого, а также все специальные сведения о разметке текста (метаданные), такие как WAV-файлы или идентификатор языка.<br/> |
| <span id="TS_IE_COMPOSITION"></span><span id="ts_ie_composition"></span><dl> <dt>**TS \_ \_Композиция IE**</dt> <dt>(0x2)</dt> </dl> | Не используется.<br/>                                                                                                                                                                  |



## <a name="remarks"></a>Комментарии

Эти константы используются в параметре *DwFlags* [ITextStoreACP:: инсертембеддед](/windows/desktop/api/Textstor/nf-textstor-itextstoreacp-insertembedded) и [итекстстореанчор:: инсертембеддед](/windows/desktop/api/Textstor/nf-textstor-itextstoreanchor-insertembedded).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                    |
| Распространяемые компоненты<br/>          | TSF 1,0 на Windows 2000 Professional<br/>                                         |
| Заголовок<br/>                   | <dl> <dt>Текстстор. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Текстстор. idl</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[ITextStoreACP:: Инсертембеддед](/windows/desktop/api/Textstor/nf-textstor-itextstoreacp-insertembedded)
</dt> <dt>

[Итекстстореанчор:: Инсертембеддед](/windows/desktop/api/Textstor/nf-textstor-itextstoreanchor-insertembedded)
</dt> </dl>

 

 





