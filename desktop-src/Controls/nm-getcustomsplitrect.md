---
title: Код уведомления NM_GETCUSTOMSPLITRECT (Коммктрл. h)
description: Отправляется элементом управления "Кнопка" в родительский элемент, чтобы получить измерения для двух прямоугольников разворачивающейся кнопки. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: ce72778d-3cca-46a4-9d05-40954a18681d
keywords:
- NM_GETCUSTOMSPLITRECT кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- NM_GETCUSTOMSPLITRECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5ab55083b830ef3ba8a0e22250d4048134fdda100bf798a8b567c13c8a949e57
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120088764"
---
# <a name="nm_getcustomsplitrect-notification-code"></a>\_Код уведомления жеткустомсплитрект (NM)

Отправляется элементом управления "Кнопка" в родительский элемент, чтобы получить измерения для двух прямоугольников разворачивающейся кнопки. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
NM_GETCUSTOMSPLITRECT
        
    nmCustomSplit = (NMCUSTOMSPLITRECTINFO *) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на [**нмкустомсплитректинфо**](/windows/win32/api/commctrl/ns-commctrl-nmcustomsplitrectinfo) для получения сведений об ограничивающих прямоугольниках. Структура **нмкустомсплитректинфо** отправляется с кодом уведомления как запрос для родителя, чтобы предоставить измерения для прямоугольников разворачивающейся кнопки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращайте [**кдрф \_ скипдефаулт**](cdrf-constants.md) , чтобы указать элементу управления "Кнопка" использовать значения, возвращаемые в структуре [**нмкустомсплитректинфо**](/windows/win32/api/commctrl/ns-commctrl-nmcustomsplitrectinfo) ; в противном случае возвратите [**кдрф \_ додефаулт**](cdrf-constants.md).

## <a name="remarks"></a>Remarks

Этот код уведомления отправляется элементом управления "Кнопка" перед его прорисовкой. Кнопка должна иметь тип [**\_ SPLITBUTTON**](button-styles.md) или [**BS \_ дефсплитбуттон**](button-styles.md). Если прямоугольники, возвращаемые элементу управления в *lParam* , недопустимы, они игнорируются.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





