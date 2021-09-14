---
description: Метод Get \_ стреаммедиатипе Извлекает тип носителя текущего потока. Все видеопотоки преобразуются в типы ВИДЕОИНФОХЕАДЕР, а все звуковые потоки преобразуются в типы ВАВЕФОРМАТЕКС.
ms.assetid: 7fc15cb3-af77-42c1-b5eb-d1d88bf9cd1d
title: 'Метод Имедиадет:: get_StreamMediaType (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMediaDet.get_StreamMediaType
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 0c2bea0c9cad7e1a25666cc38735107e14a884ec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126886904"
---
# <a name="imediadetget_streammediatype-method"></a>Метод Имедиадет:: Get \_ стреаммедиатипе

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`get_StreamMediaType`Метод извлекает тип носителя текущего потока. Все видеопотоки преобразуются в типы [**видеоинфохеадер**](/previous-versions/windows/desktop/api/amvideo/ns-amvideo-videoinfoheader) , а все звуковые потоки преобразуются в типы [**вавеформатекс**](/previous-versions/dd757713(v=vs.85)) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_StreamMediaType(
  [out, retval] AM_MEDIA_TYPE *pVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Pval* \[ out, retval\]
</dt> <dd>

Указатель на структуру [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) , которая заполнена типом носителя.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Перед вызовом этого метода задайте имя файла и поток, вызвав [**имедиадет::p UT \_ filename**](imediadet-put-filename.md) и [**имедиадет::p UT \_ куррентстреам**](imediadet-put-currentstream.md).

Если средство обнаружения мультимедиа находится в режиме захвата растрового изображения, этот метод возвращает E \_ INVALIDARG. Дополнительные сведения см. в разделе [**имедиадет:: ентербитмапграбмоде**](imediadet-enterbitmapgrabmode.md).

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Имедиадет**](imediadet.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 
