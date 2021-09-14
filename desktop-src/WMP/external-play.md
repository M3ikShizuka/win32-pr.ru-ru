---
title: Метод external. Play
description: Обратите внимание, что в этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается. метод play указывает проигрыватель Windows Media воспроизвести набор элементов мультимедиа.
ms.assetid: 3e1f45db-9e7f-4a1b-aaa2-513a19c46f70
keywords:
- метод play проигрыватель Windows Media
- метод play проигрыватель Windows Media, внешний класс
- внешний класс проигрыватель Windows Media, метод play
topic_type:
- apiref
api_name:
- External.play
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 94cfa40d96bbc67c7d41eb1a1a0188be68ec154e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241873"
---
# <a name="externalplay-method"></a>Метод external. Play

> [!Note]  
> В этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается.

 

метод **play** указывает проигрыватель Windows Media воспроизвести набор элементов мультимедиа.

## <a name="syntax"></a>Синтаксис


```JScript
External.play(
  LibraryLocationType,
  LibraryLocationIDs
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Либрарилокатионтипе* \[ окне\]
</dt> <dd>

[Константа расположения библиотеки](library-location-constants.md) , указывающая тип элементов мультимедиа для воспроизведения. Например, Кпалбумид указывает, что один или несколько альбомов должны воспроизводиться.

</dd> <dt>

*Либрарилокатионидс* \[ окне\]
</dt> <dd>

**Строка** , содержащая идентификаторы (разделенные точками с запятой) воспроизводимых элементов мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11.<br/>                                                |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Внешний объект для Интернет-магазинов типа 1**](external-object-for-type-1-online-stores.md)
</dt> </dl>

 

 





