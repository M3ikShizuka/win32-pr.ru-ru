---
title: Простые синтаксические значения SNMP (SNMP. h)
description: Простые значения синтаксиса SNMP используются для указания типа переменной SNMP.
ms.assetid: 42b681e5-721d-4d41-bc1a-c9f0005cde87
topic_type:
- apiref
api_name:
- ASN_INTEGER
- ASN_BITS
- ASN_OCTETSTRING
- ASN_NULL
- ASN_OBJECTIDENTIFIER
- ASN_INTEGER32
api_location:
- Snmp.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 85ffcd3f8e692dec2040b2b5cc86585d0ca40dd6a664c249d922eb84a16d78fb
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119886434"
---
# <a name="snmp-simple-syntax-values"></a>Простые синтаксические значения SNMP

\[Протокол SNMP доступен для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. вместо этого используйте [служба удаленного управления Windows](/windows/desktop/WinRM/portal), который является реализацией Microsoft WS-Man.\]

Простые значения синтаксиса SNMP используются для указания типа переменной SNMP.



| Константа                                                                                                                                                                           | Описание                                                           |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------|
| <span id="ASN_INTEGER"></span><span id="asn_integer"></span><dl> <dt>**ASN, \_ целое**</dt> </dl>                            | Указывает переменную с 32-битным целым числом со знаком.<br/>                |
| <span id="ASN_BITS"></span><span id="asn_bits"></span><dl> <dt>**\_биты ASN**</dt> </dl>                                     | Указывает переменную, которая является перечислением именованных битов.<br/> |
| <span id="ASN_OCTETSTRING"></span><span id="asn_octetstring"></span><dl> <dt>**ASN \_ октетстринг**</dt> </dl>                | Указывает переменную строки октета.<br/>                        |
| <span id="ASN_NULL"></span><span id="asn_null"></span><dl> <dt>**ASN \_ null**</dt> </dl>                                     | Указывает значение **null** .<br/>                                |
| <span id="ASN_OBJECTIDENTIFIER"></span><span id="asn_objectidentifier"></span><dl> <dt>**ASN \_ OBJECTIDENTIFIER**</dt> </dl> | Указывает переменную идентификатора объекта.<br/>                   |
| <span id="ASN_INTEGER32"></span><span id="asn_integer32"></span><dl> <dt>**ASN \_ INTEGER32**</dt> </dl>                      | Указывает значение 32-битового целого числа со знаком.<br/>                   |



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                        |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                              |
| Заголовок<br/>                   | <dl> <dt>Протокол SNMP. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Обзор протокола SNMP](simple-network-management-protocol-snmp-.md)
</dt> <dt>

[Справочник по SNMP](snmp-reference.md)
</dt> <dt>

[Константы SNMP](snmp-constants.md)
</dt> </dl>

 

