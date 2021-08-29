---
description: Функция-посредник для метода Инитиализепредефинед.
ms.assetid: 78137d43-c32f-4d60-b289-2e2154cf4d1e
title: Функция IWICPalette_InitializePredefined_Proxy
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWICPalette_InitializePredefined_Proxy
api_type:
- DllExport
api_location:
- Windowscodecs.dll
- Wincodec.lib
ms.openlocfilehash: 4ae1113dfba184490347bb8e255a0751884fd36c81cb8bbe337af771cd01d2ff
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119812194"
---
# <a name="iwicpalette_initializepredefined_proxy-function"></a>Ивикпалетте \_ инитиализепредефинед \_ -функция

Функция-посредник для метода [**инитиализепредефинед**](/windows/desktop/api/Wincodec/nf-wincodec-iwicpalette-initializepredefined) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IWICPalette_InitializePredefined_Proxy(
  _In_ IWICPalette          *THIS_PTR,
  _In_ WICBitmapPaletteType ePaletteType,
  _In_ BOOL                 fAddTransparentColor
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Этот \_* \[ Вход в\]
</dt> <dd>

Тип: **[ **ивикпалетте**](/windows/desktop/api/Wincodec/nn-wincodec-iwicpalette)\***

Указатель на этот объект [**ивикпалетте**](/windows/desktop/api/Wincodec/nn-wincodec-iwicpalette) .

</dd> <dt>

*епалеттетипе* \[ окне\]
</dt> <dd>

Тип: **[ **викбитмаппалеттетипе**](/windows/desktop/api/Wincodec/ne-wincodec-wicbitmappalettetype)**

Требуемый предварительно определенный тип палитры.

</dd> <dt>

*фаддтранспарентколор* \[ окне\]
</dt> <dd>

Тип: **bool** .

Необязательный цвет транпарент для добавления к палитре. Если прозрачный цвет не требуется, используйте значение 0.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если эта функция завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 2 (SP2), Windows \[ только классические приложения Vista\]<br/>                                                                                              |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                                                                             |
| DLL<br/>                      | <dl> <dt>Windowscodecs.dll; </dt> <dt>Винкодек. lib</dt> </dl> |



 

 




