---
description: Указывает средний уровень громкости звукового содержимого.
ms.assetid: eabb36ff-300f-4ed1-aca3-9415627ac1a7
title: Свойство MFPKEY_WMADRC_AVGREF (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cf18c37b00f84cc3ae3fdf1f44b2fbefcc56d9f8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460863"
---
# <a name="mfpkey_wmadrc_avgref-property"></a>МФПКЭЙ \_ вмадрк \_ Авгреф, свойство

Указывает средний уровень громкости звукового содержимого.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

g \_ всзвмадркаверажереференце

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="remarks"></a>Remarks

Это значение можно получить из кодировщика после обработки содержимого. Это значение также может быть задано для декодера в целях динамического управления диапазоном, но оно будет действовать, только если задано свойство [мфпкэй \_ вмадек \_ дркмоде](mfpkey-wmadec-drcmodeproperty.md) .

дополнительные сведения об управлении динамическими диапазонами см. в статье [Windows Media Audio Professional кодеке](/previous-versions/ms867218(v=msdn.10)).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 
