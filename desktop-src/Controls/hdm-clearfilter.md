---
title: Сообщение HDM_CLEARFILTER (Коммктрл. h)
description: Очищает фильтр для данного элемента управления "заголовок". Это сообщение можно отправить явным образом или воспользоваться заголовком \_ макроса клеарфилтер.
ms.assetid: 74c0265e-68d1-4414-8fd9-20f5f041d4b4
keywords:
- элементы управления Windows сообщений HDM_CLEARFILTER
topic_type:
- apiref
api_name:
- HDM_CLEARFILTER
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bc8b5117f7f4781bd957bf83b647cc9e4ca73cd85bda4d1a900f44c86945eca7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119436264"
---
# <a name="hdm_clearfilter-message"></a>\_Сообщение КЛЕАРФИЛТЕР HDM

Очищает фильтр для данного элемента управления "заголовок". Это сообщение можно отправить явным образом или воспользоваться [**заголовком макроса \_ клеарфилтер**](/windows/desktop/api/Commctrl/nf-commctrl-header_clearfilter) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Значение столбца, указывающее, какой фильтр следует очистить.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает целое число. **LResult** преобразуется в целое число, которое указывает **true**(1) или **false**(0).

## <a name="remarks"></a>Remarks

Если значение столбца указано как-1, удаляются все фильтры, а уведомление [ХДН \_ филтерчанже](hdn-filterchange.md) отправляется только один раз.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Клеараллфилтерс заголовка**](/windows/desktop/api/Commctrl/nf-commctrl-header_clearallfilters)
</dt> </dl>

 

 





