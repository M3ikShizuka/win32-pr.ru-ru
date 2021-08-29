---
description: Метод Сетмедиатипе задает несжатый тип носителя для группы.
ms.assetid: 51778563-f119-42e0-826b-966324a85024
title: 'Метод Иамтимелинеграуп:: Сетмедиатипе (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineGroup.SetMediaType
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 8ac32439be94234ee612bce4f3c962839099bb8239a1cfc8b48222129680d01e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120107824"
---
# <a name="iamtimelinegroupsetmediatype-method"></a>Метод Иамтимелинеграуп:: Сетмедиатипе

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetMediaType`Метод задает несжатый тип носителя для группы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetMediaType(
  [in] AM_MEDIA_TYPE *pmt
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*платежная плата* \[ окне\]
</dt> <dd>

Указатель на структуру [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) , описывающую формат.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из следующих значений **HRESULT** :



| Код возврата                                                                                             | Описание                                     |
|---------------------------------------------------------------------------------------------------------|-------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>                    | Успешно.<br/>                             |
| <dl> <dt>**\_указатель E**</dt> </dl>               | **Пустой** аргумент указателя.<br/>           |
| <dl> <dt>**VFW \_ E \_ инвалидмедиатипе**</dt> </dl> | Указан недопустимый тип носителя.<br/> |



 

## <a name="remarks"></a>Remarks

Поддерживаются следующие типы носителей:

-   Несжатое видео RGB
-   16 бит на пиксель, формат 555 (МЕДИАСУБТИПЕ \_ RGB555)
-   24 бита на пиксель (МЕДИАСУБТИПЕ \_ Rgb24)
-   32 бит на пиксель с альфа (МЕДИАСУБТИПЕ \_ ARGB32, а не медиасубтипе \_ RGB32)
-   16-разрядный стереозвук PCM (МЕДИАСУБТИПЕ \_ PCM)

Типы видео должны использовать формат \_ видеоинфо для типа формата и [**видеоинфохеадер**](/previous-versions/windows/desktop/api/amvideo/ns-amvideo-videoinfoheader) для блока Format. Формат [**VIDEOINFOHEADER2**](/previous-versions/windows/desktop/api/dvdmedia/ns-dvdmedia-videoinfoheader2) не поддерживается. Кроме того, форматы с верхними и видеороликами (*бихеигхт* < 0) не поддерживаются.

Чтобы указать формат сжатия для группы, вызовите метод [**иамтимелинеграуп:: сетсмартрекомпрессформат**](iamtimelinegroup-setsmartrecompressformat.md) .

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Интерфейс Иамтимелинеграуп**](iamtimelinegroup.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




