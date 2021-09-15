---
title: Событие Player. Аудиолангуажечанже
description: Событие Аудиолангуажечанже возникает при изменении текущего звукового языка. | Событие Player. Аудиолангуажечанже
ms.assetid: 29006a51-1b72-4fab-9906-8a0af3d92560
keywords:
- проигрыватель Windows Media событий аудиолангуажечанже
- проигрыватель Windows Media событий аудиолангуажечанже, класс Player
- класс проигрывателя проигрыватель Windows Media, событие аудиолангуажечанже
topic_type:
- apiref
api_name:
- Player.AudioLanguageChange
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e84809a966280c379f7051e500b4e385d640f890
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458259"
---
# <a name="playeraudiolanguagechange-event"></a>Событие Player. Аудиолангуажечанже

Событие **аудиолангуажечанже** возникает при изменении текущего звукового языка.

## <a name="syntax"></a>Синтаксис


```JScript
Player.AudioLanguageChange(
  LangID
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Надежно* 
</dt> <dd>

**Число** (**длинное**), определяющее новый идентификатор локали (LCID).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Код языка (LCID) однозначно определяет определенный диалект языка, который называется локальным языком.

значение параметров события задается проигрыватель Windows Media и может быть предоставлено или передано в метод в импортированном файле Microsoft JScript с использованием имени параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

**проигрыватель Windows Media 10 Mobile:** Это событие не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Controls. Куррентаудиолангуаже**](controls-currentaudiolanguage.md)
</dt> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





