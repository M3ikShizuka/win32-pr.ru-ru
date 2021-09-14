---
title: Элемент автоархивации (Чаннеллоггингтипе)
description: Определяет, следует ли создавать новый файл журнала, когда текущий файл журнала достигает максимального размера.
ms.assetid: 708c5d44-d20b-437a-a01f-6182b244c736
keywords:
- Журнал событий элемента автоархивации
topic_type:
- apiref
api_name:
- autoBackup
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 4d69c1a1c43be9d2376d94f39b3158e167f7bd13
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885485"
---
# <a name="autobackup-channelloggingtype-element"></a>Элемент автоархивации (Чаннеллоггингтипе)

Определяет, следует ли создавать новый файл журнала, когда текущий файл журнала достигает максимального размера.

``` syntax
<xs:element name="autoBackup"
    type="boolean"
 />
```

Элемент **автоархивации** определяется сложным типом [**чаннеллоггингтипе**](eventmanifestschema-channelloggingtype-complextype.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Родительский элемент**
</dt> <dt>

[**ведение журнала (Чаннелтипе)**](eventmanifestschema-logging-channeltype-element.md)
</dt> </dl>

 

 





