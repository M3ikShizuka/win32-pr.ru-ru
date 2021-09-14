---
title: Метод Controls. Step
description: Метод Step заставляет текущий видеоматериал закреплять воспроизведение на следующем кадре или предыдущем кадре.
ms.assetid: f717c583-4073-45a9-b05d-7134d02724a4
keywords:
- проигрыватель Windows Media метода step
- метод step проигрыватель Windows Media, класс controls
- класс элементов управления проигрыватель Windows Media, метод step
topic_type:
- apiref
api_name:
- Controls.step
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 43fc50ea28bde95efef6e6261788fdcc62df6089
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967674"
---
# <a name="controlsstep-method"></a>Метод Controls. Step

Метод **Step** заставляет текущий видеоматериал закреплять воспроизведение на следующем кадре или предыдущем кадре.

## <a name="syntax"></a>Синтаксис


```JScript
Controls.step(
  frameCount
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*фрамекаунт* \[ окне\]
</dt> <dd>

**Число** (**длинное**), указывающее, сколько кадров следует пошагово перед замораживанием. В настоящее время необходимо задать значение 1 или-1.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

В настоящее время этот метод поддерживает только параметры 1 или-1, поэтому каждый раз можно пошаговым образом выполнять только один кадр.

**проигрыватель Windows Media 10 Mobile:** Этот метод не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media для Windows XP или более поздней версии.<br/>                           |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Controls**](controls-object.md)
</dt> <dt>

[**Объект DVD**](dvd-object.md)
</dt> </dl>

 

 





