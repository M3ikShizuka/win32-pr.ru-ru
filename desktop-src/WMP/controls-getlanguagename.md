---
title: Controls. Жетлангуаженаме, метод
description: Метод Жетлангуаженаме извлекает имя звукового языка с указанным кодом локали (LCID).
ms.assetid: 9e142c89-92bf-476f-bae7-b94f5b5ebe01
keywords:
- проигрыватель Windows Media метода жетлангуаженаме
- проигрыватель Windows Media метода жетлангуаженаме, класс controls
- класс элементов управления проигрыватель Windows Media, метод жетлангуаженаме
topic_type:
- apiref
api_name:
- Controls.getLanguageName
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e747860c60313a66eecf8b7d6bd289ffb47f282c8c8d7633716e5c4e60ca7674
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118997484"
---
# <a name="controlsgetlanguagename-method"></a>Controls. Жетлангуаженаме, метод

Метод **жетлангуаженаме** извлекает имя звукового языка с указанным кодом локали (LCID).

## <a name="syntax"></a>Синтаксис


```JScript
strRetVal = Controls.getLanguageName(
  LCID
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Код языка* \[ в\]
</dt> <dd>

**Число** (**длинное**), определяющее код языка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **строку**.

## <a name="remarks"></a>Remarks

Код языка (LCID) однозначно определяет определенный диалект языка, который называется локальным языком.

для Windows содержимого на основе носителя свойства и методы, связанные с выбором языка, поддерживают только один выход.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Controls**](controls-object.md)
</dt> <dt>

[**Controls. Аудиолангуажекаунт**](controls-audiolanguagecount.md)
</dt> <dt>

[**Controls. Куррентаудиолангуаже**](controls-currentaudiolanguage.md)
</dt> <dt>

[**Controls. Куррентаудиолангуажеиндекс**](controls-currentaudiolanguageindex.md)
</dt> <dt>

[**Controls. Жетаудиолангуажедескриптион**](controls-getaudiolanguagedescription.md)
</dt> <dt>

[**Controls. Жетаудиолангуажеид**](controls-getaudiolanguageid.md)
</dt> </dl>

 

 





