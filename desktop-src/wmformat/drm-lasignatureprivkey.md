---
title: DRM_LASignaturePrivKey
description: Свойство DRM \_ ласигнатурепривкэй содержит закрытый ключ, используемый для шифрования заголовка DRM.
ms.assetid: b7083237-da11-4f31-a143-c0278a54b5a6
keywords:
- DRM_LASignaturePrivKey формат Windows Media
topic_type:
- apiref
api_name:
- DRM_LASignaturePrivKey
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1cdb22f3abc57fc2331ff87bd05bc05d580d607c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127345462"
---
# <a name="drm_lasignatureprivkey"></a>\_ЛАСИГНАТУРЕПРИВКЭЙ DRM

Свойство **DRM \_ ласигнатурепривкэй** содержит закрытый ключ, используемый для шифрования заголовка DRM.

## <a name="global-constant"></a>Глобальная константа

g \_ всзвмдрм \_ ласигнатурепривкэй

## <a name="data-type"></a>Тип данных

**\_Строка типа \_ ВМТ**

## <a name="remarks"></a>Remarks

Это свойство может быть создано с помощью метода [**ивмдрмвритер:: женератесигнингкэйпаир**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmdrmwriter-generatesigningkeypair) . Это свойство должно оставаться секретом, известным только создателю содержимого. Это свойство можно задать с помощью метода [**ивмдрмвритер:: сетдрматтрибуте**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmdrmwriter-setdrmattribute) . Он недоступен для объекта Reader.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Список атрибутов**](attribute-list.md)
</dt> </dl>

 

 




