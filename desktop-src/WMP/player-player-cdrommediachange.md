---
title: Событие Player. Кдроммедиачанже
description: Событие Кдроммедиачанже возникает при вставке или извлечении компакт-диска или DVD-диска из дисковода CD или DVD. | Событие Player. Кдроммедиачанже
ms.assetid: d31a791a-55e5-49ee-bfe5-7488277e3fda
keywords:
- проигрыватель Windows Media событий кдроммедиачанже
- проигрыватель Windows Media событий кдроммедиачанже, класс Player
- класс проигрывателя проигрыватель Windows Media, событие кдроммедиачанже
topic_type:
- apiref
api_name:
- Player.CdromMediaChange
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3c3125235d5f8d19963b85284e7dbe40c7af408d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342787"
---
# <a name="playercdrommediachange-event"></a>Событие Player. Кдроммедиачанже

Событие **кдроммедиачанже** возникает при вставке или ИЗВЛЕЧЕНии компакт-диска или DVD-диска из дисковода CD или DVD.

## <a name="syntax"></a>Синтаксис


```JScript
Player.CdromMediaChange(
  CdromNum
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*кдромнум* 
</dt> <dd>

**Число** (**длинное**), указывающее индекс компакт-диска или DVD-дисковода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Индекс дисковода компакт-дисков соответствует индексу объекта **CDROM** в **кдромколлектион**.

значение параметров события задается проигрыватель Windows Media, и к нему можно получить доступ или передать в метод в импортированном JScriptном файле, используя имя параметра. Имя этого параметра должно быть введено в точности так, как показано, включая прописные буквы.

**проигрыватель Windows Media 10 Mobile:** Это событие не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект CDROM**](cdrom-object.md)
</dt> <dt>

[**Объект Кдромколлектион**](cdromcollection-object.md)
</dt> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





