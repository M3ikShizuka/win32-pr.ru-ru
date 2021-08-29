---
title: THEME. Лоадпреференце
description: Метод Лоадпреференце загружает предпочтение из реестра.
ms.assetid: 51d6b0f8-f1fd-4999-a575-0b7c177b2bc8
keywords:
- проигрыватель Windows Media THEME. лоадпреференце
topic_type:
- apiref
api_name:
- THEME.loadPreference
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 252f08c1971b1e8434e3761d87992a7245257c37bcc039650ebf5b7a0a47a884
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119134577"
---
# <a name="themeloadpreference"></a>THEME. Лоадпреференце

Метод **лоадпреференце** загружает предпочтение из реестра.

``` syntax
        theme.loadPreference(theKey)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="theKey"></span><span id="thekey"></span><span id="THEKEY"></span>*секэй*
</dt> <dd>

**Строка** , указывающая ключ значения предпочтения для загрузки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **строку**.

## <a name="remarks"></a>Remarks

предпочтение — это пара "ключ-значение", которая может храниться в реестре для сохранения сведений о состоянии проигрыватель Windows Media между запусками. эта функция может использоваться, например, для сохранения параметров настройки, чтобы их не нужно было повторно указывать при каждом запуске проигрыватель Windows Media.

Параметры не шифруются и поэтому не являются безопасным методом для сохранения данных. Не используйте настройки для хранения частных данных.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент THEME**](theme-element.md)
</dt> <dt>

[**THEME. Савепреференце**](theme-savepreference.md)
</dt> </dl>

 

 





