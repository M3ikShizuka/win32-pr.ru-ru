---
description: Метод Get \_ mediaType возвращает текущий тип выходного носителя фильтра.
ms.assetid: b9900f7c-05f6-47e4-9cb0-683df2aea404
title: 'Метод Иресизе:: get_MediaType (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IResize.get_MediaType
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: b03bad7f8686fd580f7dd5fc347c347ade1c1c97
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891768"
---
# <a name="iresizeget_mediatype-method"></a>Метод Иресизе:: Get \_ mediaType

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`get_MediaType`Метод возвращает текущий тип выходного носителя фильтра.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_MediaType(
  [out] AM_MEDIA_TYPE *pmt
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*платежная плата* \[ заполняет\]
</dt> <dd>

Указатель на структуру [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) , выделенную вызывающей стороной. Метод заполняет эту структуру типом мультимедиа. Вызывающий объект должен освободить блок формата, если таковой имеется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Если тип выходного носителя не задан, возвращается тип носителя по умолчанию. Фильтр должен обновить тип выходного носителя, когда вызываются методы **размещения \_ mediaType** или Where **\_ size** ; тип носителя, возвращаемый методом, `get_MediaType` должен отражать эти изменения.

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | DirectX 9,0 или более поздней версии<br/>                                                         |
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> <dt>

[**Интерфейс Иресизе**](iresize.md)
</dt> </dl>

 

 




