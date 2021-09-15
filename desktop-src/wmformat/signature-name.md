---
title: Signature_Name
description: '\_Атрибут имени подписи содержит имя сертификата, используемого для подписания файла. Этот атрибут допустим только в том случае, если \_ атрибуту является Trusted задано значение true.'
ms.assetid: 3f3ab10c-731b-4075-8f73-3c2e62e010b9
keywords:
- Signature_Name формат Windows Media
topic_type:
- apiref
api_name:
- Signature_Name
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: af378671a570dd9ffc58021081b3925d3dca21af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570203"
---
# <a name="signature_name"></a>\_Имя подписи

Атрибут **\_ имени подписи** содержит имя сертификата, используемого для подписания файла. Этот атрибут допустим только в том случае, если атрибуту [**является \_ Trusted**](is-trusted.md) задано значение true.

## <a name="global-constant"></a>Глобальная константа

\_всзвмсигнатуре \_ имя

## <a name="data-type"></a>Тип данных

**\_Строка типа \_ ВМТ**

## <a name="remarks"></a>Remarks

Это закодированный атрибут.

Этот атрибут не может дублироваться на уровне файла. если этот атрибут используется для отдельного потока, он будет рассматриваться как пользовательские метаданные и не будет передавать свое нормальное значение объектам из пакета SDK Windows Media Format.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Список атрибутов**](attribute-list.md)
</dt> </dl>

 

 




