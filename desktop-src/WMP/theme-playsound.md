---
title: THEME. playSound
description: Метод playSound воспроизводит указанный звуковой файл.
ms.assetid: 42675a66-0139-4e74-9abe-1b42017fc6fe
keywords:
- THEME. playSound проигрыватель Windows Media
topic_type:
- apiref
api_name:
- THEME.playSound
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 8ceb30e5c47632a1358262019124fceae056294d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168604"
---
# <a name="themeplaysound"></a>THEME. playSound

Метод **PlaySound** воспроизводит указанный звуковой файл.

``` syntax
        theme.playSound(soundFile)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="soundFile"></span><span id="soundfile"></span><span id="SOUNDFILE"></span>*soundFile*
</dt> <dd>

**Строка** , указывающая имя звукового файла для воспроизведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод позволяет добавлять звуковые эффекты к обложке, например при нажатии кнопок. звук воспроизводится операционной системой напрямую, а не проигрыватель Windows Media. это означает, что звук не может управляться с помощью параметров проигрыватель Windows Media и методов, но его можно воспроизводить, когда проигрыватель Windows Media воспроизводит другой файл цифрового мультимедиа.

Этот метод поддерживает только файлы WAV.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент THEME**](theme-element.md)
</dt> </dl>

 

 





