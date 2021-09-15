---
description: возвращает родительский элемент в дереве, представляющий устройство Windowsного устройства получения изображений (WIA) 2,0.
ms.assetid: c6fdaf1d-9875-4852-893c-813894d89f6c
title: 'Метод IWiaItem2:: Жетпарентитем (WIA. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWiaItem2.GetParentItem
api_type:
- COM
api_location:
- Wia.h
ms.openlocfilehash: 055625b98807103c3b79109216f6081d00564b15
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572286"
---
# <a name="iwiaitem2getparentitem-method"></a>Метод IWiaItem2:: Жетпарентитем

возвращает родительский элемент в дереве, представляющий устройство Windowsного устройства получения изображений (WIA) 2,0.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetParentItem(
  [out] IWiaItem2 **ppIWiaItem2
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ppIWiaItem2* \[ заполняет\]
</dt> <dd>

Тип: **[ **IWiaItem2**](-wia-iwiaitem2.md)\*\***

Получает адрес указателя на интерфейс [**IWiaItem2**](-wia-iwiaitem2.md) родителя элемента в дереве объектов элементов. Если этот метод вызывается в корне дерева, возвращенный адрес имеет **значение NULL**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

При наличии объекта [**IWiaItem2**](-wia-iwiaitem2.md) в дереве объектов аппаратного устройства WIA 2,0 приложение получает указатель на родительский элемент, вызывая эту функцию.

Приложения должны вызывать метод [IUnknown:: Release](/windows/win32/api/unknwn/nf-unknwn-iunknown-release) для указателей интерфейса, которые они получают через параметр *ppIWiaItem2* , если эти указатели не **равны NULL**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>WIA. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>WIA. idl</dt> </dl> |



 

 
