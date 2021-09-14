---
title: Сообщение PSM_SETHEADERTITLE (Пршт. h)
description: Задает текст заголовка для заголовка внутренней страницы мастера. Это сообщение можно отправить явным образом или использовать макрос Пропшит \_ сесеадертитле.
ms.assetid: 19d4badf-d99d-4a28-92d4-33bcf5d23944
keywords:
- элементы управления Windows сообщений PSM_SETHEADERTITLE
topic_type:
- apiref
api_name:
- PSM_SETHEADERTITLE
- PSM_SETHEADERTITLEA
- PSM_SETHEADERTITLEW
api_location:
- Prsht.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8140eef4aa09e9dd19d8baaf8193a836b105482e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167483"
---
# <a name="psm_setheadertitle-message"></a>\_Сообщение ПСМ сесеадертитле

Задает текст заголовка для заголовка внутренней страницы мастера. Это сообщение можно отправить явным образом или использовать макрос [**пропшит \_ сесеадертитле**](/windows/desktop/api/Prsht/nf-prsht-propsheet_setheadertitle) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Отсчитываемый от нуля индекс страницы мастера.

</dd> <dt>

*lParam* 
</dt> <dd>

Подзаголовок нового заголовка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Если указать текущую страницу, она будет немедленно перерисована для вывода нового заголовка.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>Пршт. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ПСМ \_ СЕСЕАДЕРТИТЛЕВ** (Юникод) и **ПСМ \_ сесеадертитлеа** (ANSI)<br/>  |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**ПСМ \_ хвндтоиндекс**](psm-hwndtoindex.md)
</dt> <dt>

[**ПСМ \_ идтоиндекс**](psm-idtoindex.md)
</dt> <dt>

[**ПСМ \_ пажетоиндекс**](psm-pagetoindex.md)
</dt> </dl>

 

 





