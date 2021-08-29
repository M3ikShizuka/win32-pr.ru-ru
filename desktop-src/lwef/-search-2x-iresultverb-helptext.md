---
title: Свойство HelpText Иресултверб (Вдсшаредидл. h)
description: Это свойство возвращает указатель на локализованную строку справки для команды.
ms.assetid: 14e91101-5ee2-459a-97d7-35c76d3ba990
keywords:
- свойства HelpText устаревшие Windows функции среды
- свойства HelpText устаревшие Windows функции среды, интерфейс иресултверб
- интерфейс иресултверб устаревшие функции среды Windows, свойство HelpText
topic_type:
- apiref
api_name:
- IResultVerb.HelpText
- IResultVerb.get_HelpText
api_location:
- WdsSharedIDL.h
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d314e9cd84382449273ddbfb0ee54ae9b6c7aa1fdb528cc33db4a85abd5ce02d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120014314"
---
# <a name="iresultverbhelptext-property"></a>Свойство Иресултверб:: HelpText

> [!NOTE]
> Windows настольный поиск 2. x — это устаревшая технология, которая изначально была доступна в качестве надстройки для Windows XP и Windows Server 2003. в более поздних выпусках используйте вместо этого [API Windows поиска](../search/-search-reference-entry-page.md) . 

Это свойство возвращает указатель на локализованную строку справки для команды.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_HelpText(
  [out, retval] BSTR *text
);
```



## <a name="property-value"></a>Значение свойства

Значение этого свойства является указателем на локализованную строку справки для этой команды.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 2 (SP2) \[ только классические приложения\]<br/>                                      |
| Минимальная версия сервера<br/> | Windows Только для настольных приложений сервера 2003 с пакетом обновления 1 \[\]<br/>                             |
| Распространяемые компоненты<br/>          | Windows Поиск на рабочем столе (WDS) 2.6.5<br/>                                             |
| Заголовок<br/>                   | <dl> <dt>Вдсшаредидл. h</dt> </dl> |



 

 





