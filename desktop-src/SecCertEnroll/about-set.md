---
description: НАБОР содержит неупорядоченную последовательность полей одного или нескольких типов.
ms.assetid: 6bbe89da-1177-4cfa-9515-03b271e5ef6b
title: SET
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 95eb2b9df8097f716ef98d55d052d2dbc2ef09b1bfe57de0e793d2b063967710
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118903683"
---
# <a name="set"></a>SET

**Набор** содержит неупорядоченную последовательность полей одного или нескольких типов. Он кодируется в TLV-Triplet, который начинается с **тега** Byte 0x31. В следующем примере, преобразованном из раздела [ASN. 1 в формате CMC](cmc-encoded-asn-1.md) , показано, как атрибут **ClientID** кодируется в структуре данных **набора** . Атрибут можно указать с помощью интерфейса [**IX509AttributeClientId**](/windows/desktop/api/CertEnroll/nn-certenroll-ix509attributeclientid) .

``` syntax
31 59                                     ; SET (59 Bytes)
   30 57                                  ; SEQUENCE (57 Bytes)
      06 09                               ; OBJECT_ID (9 Bytes)
      |  2b 06 01 04 01 82 37 15  14      ;   1.3.6.1.4.1.311.21.20 
      31 4a                               ; SET (4a Bytes)
         30 48                            ; SEQUENCE (48 Bytes)
            02 01                         ; INTEGER (1 Bytes)
            |  09
            0c 23                         ; UTF8_STRING (23 Bytes)
            |  76 69 63 68 33 64 2e 6a    ;   vich3d.j
            |  64 6f 6d 63 73 63 2e 6e    ;   domcsc.n
            |  74 74 65 73 74 2e 6d 69    ;   ttest.mi
            |  63 72 6f 73 6f 66 74 2e    ;   crosoft.
            |  63 6f 6d                   ;   com
            0c 15                         ; UTF8_STRING (15 Bytes)
            |  4a 44 4f 4d 43 53 43 5c    ;   JDOMCSC\
            |  61 64 6d 69 6e 69 73 74    ;   administ
            |  72 61 74 6f 72             ;   rator
            0c 07                         ; UTF8_STRING 
```

Если **набор** содержит менее 128 байт, поле **length** TLV Triplet требует только одного байта для указания длины содержимого. Если его длина превышает 127 байт, в поле **length** в разряде 7 устанавливается значение 1, а для битов с 6 по 0 укажите число дополнительных байтов, используемых для определения длины содержимого. Дополнительные сведения см. в разделе [кодированная Длина и байты значений](about-encoded-length-and-value-bytes.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Система типов ASN. 1](about-asn-1-type-system.md)
</dt> <dt>

[Кодировка DER для типов ASN. 1](about-der-encoding-of-asn-1-types.md)
</dt> </dl>

 

 



