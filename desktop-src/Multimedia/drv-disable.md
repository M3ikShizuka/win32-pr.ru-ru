---
title: Сообщение DRV_DISABLE (Ммсистем. h)
description: Отключает драйвер. Драйвер должен разместить соответствующее устройство (если оно имеется) в неактивном состоянии и завершить любые функции обратного вызова или потоки.
ms.assetid: 83e99397-6f0e-4174-9f96-e10c1f17ef0b
keywords:
- сообщение DRV_DISABLE Windows мультимедиа
topic_type:
- apiref
api_name:
- DRV_DISABLE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b512e90612a02681008474c7f1323f17304422d2
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370461"
---
# <a name="drv_disable-message"></a>DRV \_ отключить сообщение

Отключает драйвер. Драйвер должен разместить соответствующее устройство (если оно имеется) в неактивном состоянии и завершить любые функции обратного вызова или потоки.

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="hdrvr"></span><span id="HDRVR"></span>*хдрвр*
</dt> <dd>

Описатель устанавливаемого экземпляра драйвера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Параметры *двдриверид*, *lParam1* и *lParam2* не используются.

После отключения драйвера система обычно отправляет драйверу краткое сообщение [**DRV \_**](drv-free.md) , прежде чем удалить драйвер из памяти.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Устанавливаемые драйверы](installable-drivers.md)
</dt> <dt>

[Устанавливаемые сообщения драйверов](installable-driver-messages.md)
</dt> </dl>

 

 





