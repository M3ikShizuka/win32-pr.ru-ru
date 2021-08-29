---
description: Метод Сетдефаултфпс задает частоту кадров исходного объекта по умолчанию.
ms.assetid: ea93acde-3e05-43d5-8130-9ab2ee841b4e
title: 'Метод Иамтимелинесрк:: Сетдефаултфпс (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineSrc.SetDefaultFPS
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 5eda06b5aeb327de21b72332cd26a71884369b9c4171e1b0611f0e6259f9c1ce
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119915014"
---
# <a name="iamtimelinesrcsetdefaultfps-method"></a>Метод Иамтимелинесрк:: Сетдефаултфпс

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetDefaultFPS`Метод задает частоту кадров исходного объекта по умолчанию.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetDefaultFPS(
   double FPS
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Кадры в секунду* 
</dt> <dd>

Частота кадров по умолчанию в кадрах в секунду.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ ОК в случае успеха или E \_ INVALIDARG, если указанная частота кадров меньше нуля.

## <a name="remarks"></a>Remarks

Модуль подготовки отчетов использует это значение, если не может определить частоту кадров из исходного файла.

Вызывайте этот метод только для исходных файлов без стандартной частоты кадров. Для растровых и JPEG-файлов частота кадров по умолчанию равна нулю, что приводит к отображению источника в виде изображения по-прежнему. Чтобы использовать изображение в качестве первого кадра в последовательности DIB, задайте для параметра Частота кадров значение больше нуля. Дополнительные сведения см. в разделе [Работа с источниками](working-with-sources.md).

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

[**Интерфейс Иамтимелинесрк**](iamtimelinesrc.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




