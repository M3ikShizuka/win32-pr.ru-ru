---
description: Фильтрует изображение предварительного просмотра.
ms.assetid: 1710211a-a35c-4a51-b3bb-6f03f234f247
title: 'Метод Ивиаимажефилтер:: Филтерпревиевимаже (WIA. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IWiaImageFilter.FilterPreviewImage
api_type:
- COM
api_location:
- Wia.h
ms.openlocfilehash: 882aaf0d131ae6fe062c00c0181e2f913a0e1bc5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572290"
---
# <a name="iwiaimagefilterfilterpreviewimage-method"></a>Метод Ивиаимажефилтер:: Филтерпревиевимаже

Фильтрует изображение предварительного просмотра.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT FilterPreviewImage(
  [in] LONG      lFlags,
  [in] IWiaItem2 *pWiaChildItem2,
  [in] RECT      InputImageExtents,
  [in] IStream   *pInputStream
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*лфлагс* \[ окне\]
</dt> <dd>

Тип: **Long**

Не используется. Задайте значение 0.

</dd> <dt>

*pWiaChildItem2* \[ окне\]
</dt> <dd>

Тип: **[ **IWiaItem2**](-wia-iwiaitem2.md)\***

Обрабатываемый элемент.

</dd> <dt>

*Инпутимажеекстентс* \[ окне\]
</dt> <dd>

Тип: **Rect**

Координаты (в области физического приобретения) образа, который компонент предварительной версии кэширует внутренне.

</dd> <dt>

*пинпутстреам* \[ окне\]
</dt> <dd>

Тип: **[IStream](/windows/win32/api/objidl/nn-objidl-istream)\***

Указатель на интерфейс [IStream](/windows/win32/api/objidl/nn-objidl-istream) для фильтруемых данных изображения в кэше.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Не вызывайте этот метод непосредственно из приложения.

*pWiaChildItem2* должен быть дочерним элементом *pWiaItem2* , переданным в [**ивиаимажефилтер:: инитиализефилтер**](-wia-iwiaimagefilter-initializefilter.md).

*Инпутимажеекстентс* требуется, поскольку фильтр обработки изображений отвечает за Вырезание области изображения, которую *pWiaChildItem2* представляет из данных изображения, передаваемых через *пинпутстреам*.

Приложение должно гарантировать, что *pWiaChildItem2* имеет тот же формат изображения ( \_ Формат WIA IPA \_ ), разрешение (с помощью WIA-пакетов \_ \_ ксрес и WIA \_ \_ -адресов ИРЕС) и глубину ( \_ глубину WIA IPA \_ ) в качестве *pWiaItem2* при передаче в [**жетневпревиев**](-wia-iwiapreview-getnewpreview.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                     |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                               |
| Заголовок<br/>                   | <dl> <dt>WIA. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>WIA. idl</dt> </dl> |



 

 
