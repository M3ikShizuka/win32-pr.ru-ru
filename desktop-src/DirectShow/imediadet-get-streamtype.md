---
description: Метод Get \_ стреамтипе извлекает глобальный уникальный идентификатор (GUID) для типа мультимедиа текущего потока.
ms.assetid: 2f61b3fe-c041-4031-9211-2f5fc189542b
title: 'Метод Имедиадет:: get_StreamType (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMediaDet.get_StreamType
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 1a027059854ba02e4a846660435731f140b6d04cb8d96f714fd63f1d24757ca1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120083724"
---
# <a name="imediadetget_streamtype-method"></a>Метод Имедиадет:: Get \_ стреамтипе

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`get_StreamType`Метод получает Глобальный уникальный идентификатор (GUID) для типа мультимедиа текущего потока.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_StreamType(
  [out, retval] GUID *pVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Pval* \[ out, retval\]
</dt> <dd>

Получает основной GUID типа для типа мультимедиа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Этот метод извлекает элемент **мажортипе** структуры [**\_ \_ типа мультимедиа AM**](/windows/win32/api/strmif/ns-strmif-am_media_type) . Структура **\_ \_ типа мультимедиа AM** описывает формат потока, а элемент **мажортипе** — идентификатор GUID, указывающий общую категорию, например аудио или видео. Для потока видео GUID — это видео типа MEDIATYPE \_ . Для звукового сигнала используется параметр MEDIATYPE \_ Audio. Чтобы получить всю структуру **\_ \_ типа мультимедиа AM** , вызовите метод [**имедиадет:: Get \_ стреаммедиатипе**](imediadet-get-streammediatype.md) .

Перед вызовом этого метода задайте имя файла и поток, вызвав [**имедиадет::p UT \_ filename**](imediadet-put-filename.md) и [**имедиадет::p UT \_ куррентстреам**](imediadet-put-currentstream.md).

Если средство обнаружения мультимедиа находится в режиме захвата растрового изображения, этот метод возвращает E \_ INVALIDARG. Дополнительные сведения см. в разделе [**имедиадет:: ентербитмапграбмоде**](imediadet-enterbitmapgrabmode.md).

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Интерфейс Имедиадет**](imediadet.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




