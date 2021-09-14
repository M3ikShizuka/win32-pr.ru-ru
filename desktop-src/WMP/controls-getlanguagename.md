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
ms.openlocfilehash: 798a6b22f344953df716e4df4ed8a9a0daff2a7b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967701"
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

## <a name="remarks"></a>Комментарии

Код языка (LCID) однозначно определяет определенный диалект языка, который называется локальным языком.

для Windows содержимого на основе носителя свойства и методы, связанные с выбором языка, поддерживают только один выход.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

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

 

 





