---
description: 'Метод Сетдефаултфпс задает частоту выходного кадра по умолчанию в кадрах в секунду. Группы используют это значение в качестве частоты кадров по умолчанию. Чтобы задать частоту кадров группы, вызовите метод Иамтимелинеграуп:: Сетаутпутфпс в группе.'
ms.assetid: a164f4b9-fbed-45ea-9156-cc64f0b21423
title: 'Метод Иамтимелине:: Сетдефаултфпс (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimeline.SetDefaultFPS
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 20c352f40234672ceeb2d4c25ea9db04e89f712d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126892240"
---
# <a name="iamtimelinesetdefaultfps-method"></a>Метод Иамтимелине:: Сетдефаултфпс

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetDefaultFPS`Метод задает частоту выходного кадра по умолчанию в кадрах в секунду. Группы используют это значение в качестве частоты кадров по умолчанию. Чтобы задать частоту кадров группы, вызовите метод [**иамтимелинеграуп:: сетаутпутфпс**](iamtimelinegroup-setoutputfps.md) в группе.

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

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

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

[**Интерфейс Иамтимелине**](iamtimeline.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




