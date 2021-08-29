---
description: Указывает предпочтительное количество выборок на кадр.
ms.assetid: ad629dbd-49d8-43d0-95a8-03f2043e397e
title: Свойство MFPKEY_PREFERRED_FRAMESIZE (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a82fbc234235d0caf46b5c1a0fa3278fc98b174db318a894d735ec2878492de9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119463244"
---
# <a name="mfpkey_preferred_framesize-property"></a>МФПКЭЙ \_ предпочтительное \_ свойство фрамесизе

Указывает предпочтительное количество выборок на кадр.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

**VT \_ UI4**

## <a name="remarks"></a>Remarks

Чтобы задать предпочтительный размер кадра, задайте следующие свойства.

-   Задайте [**для \_ мфпкэй \_ запрос \_ фрамесизе**](mfpkey-requesting-a-framesizeproperty.md) к **варианту \_ true**.
-   Задайте для параметра **мфпкэй \_ предпочтительный \_ фрамесизе** число выборок в каждом кадре.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|-----------------------------------------------------------------------------------------|
| Клиент<br/> | Windows Vista или Windows 7<br/>                                                   |
| Header<br/> | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 
