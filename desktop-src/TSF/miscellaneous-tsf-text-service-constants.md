---
title: Различные константы службы текстового ввода TSF (Ктффунк. h)
description: В текстовых службах используются следующие значения.
ms.assetid: 38110314-1638-4963-92b6-4ba2f81fb7c2
topic_type:
- apiref
api_name:
- TF_MENUREADY
- TF_PROPUI_STATUS_SAVETOFILE
api_location:
- Ctffunc.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d7ebd7d22f9cfbd59f95ee3dcfe68229536503b0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170735"
---
# <a name="miscellaneous-tsf-text-service-constants"></a>Различные константы службы текстового ввода TSF

В текстовых службах используются следующие значения.



| Константа/значение                                                                                                                                                                                                                                                            | Описание                                                                                                                                                                                                                                                                              |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="TF_MENUREADY"></span><span id="tf_menuready"></span><dl> <dt>**Tf \_ МЕНУРЕАДИ**</dt> <dt>0x00000001</dt> </dl>                                                | В настоящий момент не используется.<br/>                                                                                                                                                                                                                                                           |
| <span id="TF_PROPUI_STATUS_SAVETOFILE"></span><span id="tf_propui_status_savetofile"></span><dl> <dt>**Tf \_ \_Состояние пропуи \_ SAVETOFILE**</dt> <dt>0x00000001</dt> </dl> | Свойство может быть сериализовано. Если это значение отсутствует, свойство не может быть сериализовано. Это значение используется с [итффнпропертюистатус::-Status](/windows/desktop/api/Ctffunc/nf-ctffunc-itffnpropertyuistatus-getstatus) и [Итффнпропертюистатус:: SetStatus](/windows/desktop/api/Ctffunc/nf-ctffunc-itffnpropertyuistatus-setstatus).<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                             |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                   |
| Распространяемые компоненты<br/>          | TSF 1,0 на Windows 2000 Professional<br/>                                        |
| Заголовок<br/>                   | <dl> <dt>Ктффунк. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Ктффунк. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Итффнпропертюистатус::/Status](/windows/desktop/api/Ctffunc/nf-ctffunc-itffnpropertyuistatus-getstatus)
</dt> <dt>

[Итффнпропертюистатус:: SetStatus](/windows/desktop/api/Ctffunc/nf-ctffunc-itffnpropertyuistatus-setstatus)
</dt> </dl>

 

 





