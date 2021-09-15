---
description: Включает фильтр обработки изображений для записи свойств обратно в драйвер (и на устройство).
ms.assetid: b9bb8d81-2945-46ba-a0a2-7009000574aa
title: 'Метод Ивиаимажефилтер:: Апплипропертиес (WIA. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWiaImageFilter.ApplyProperties
api_type:
- COM
api_location:
- Wia.h
ms.openlocfilehash: 3c20527ee587b975adea34e7c480349836620015
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572291"
---
# <a name="iwiaimagefilterapplyproperties-method"></a>Метод Ивиаимажефилтер:: Апплипропертиес

Включает фильтр обработки изображений для записи свойств обратно в драйвер (и на устройство).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ApplyProperties(
  [in] IWiaPropertyStorage *pWiaPropertyStorage
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пвиапропертистораже* \[ окне\]
</dt> <dd>

Тип: **[ **ивиапропертистораже**](/windows/desktop/api/wia_xp/nn-wia_xp-iwiapropertystorage)\***

Указывает указатель на [**ивиапропертистораже**](/windows/desktop/api/wia_xp/nn-wia_xp-iwiapropertystorage) для применения свойств.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Не вызывайте этот метод непосредственно из приложения. он вызывается Windows получения образа (WIA) 2,0 после того, как фильтр обработки изображений обработал необработанные данные.

*пвиапропертистораже* — это интерфейс [**ивиапропертистораже**](/windows/desktop/api/wia_xp/nn-wia_xp-iwiapropertystorage) , в который фильтр обработки изображений должен записывать свойства. Фильтр обработки изображений должен использовать только метод [ипропертистораже:: вритемултипле](/windows/win32/api/propidlbase/nf-propidlbase-ipropertystorage-writemultiple) для записи свойств.

Этот метод позволяет фильтру обработки изображений записывать свойства обратно в драйвер (и на устройство). Это может потребоваться для фильтров, которые реализуют такие функции, как автоматическая раскрытие во время сканирования пленки.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>WIA. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>WIA. idl</dt> </dl> |



 

 
