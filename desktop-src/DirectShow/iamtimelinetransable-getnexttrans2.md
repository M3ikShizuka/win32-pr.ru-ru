---
description: 'Метод GetNextTrans2 извлекает первый переход, который отображается в указанное время или позже. Этот метод эквивалентен Иамтимелинетрансабле:: Жетнексттранс, но принимает значение РЕФТИМЕ.'
ms.assetid: e6910e94-f289-4a5d-9976-1e8f7373c882
title: 'Метод Иамтимелинетрансабле:: GetNextTrans2 (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineTransable.GetNextTrans2
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 9c3b1fbc45ca4407e1305704cf40fc82259194d46b270ececf8e5f5d3211b99d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119965064"
---
# <a name="iamtimelinetransablegetnexttrans2-method"></a>Метод Иамтимелинетрансабле:: GetNextTrans2

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`GetNextTrans2`Метод извлекает первый переход, который отображается в указанное время или позже. Этот метод эквивалентен [**иамтимелинетрансабле:: жетнексттранс**](iamtimelinetransable-getnexttrans.md), но принимает значение [**рефтиме**](reftime.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetNextTrans2(
  [out] IAMTimelineObj **ppTrans,
        REFTIME        *pInOut
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пптранс* \[ заполняет\]
</dt> <dd>

Получает указатель на интерфейс [**иамтимелинеобж**](iamtimelineobj.md) объекта перехода.

</dd> <dt>

*\Sub* 
</dt> <dd>

Указатель на переменную, указывающую время в секундах. В поле входное значение указывает время, с которого нужно найти переход. В выходных данных, если переход получен, это значение устанавливается равным времени окончания перехода.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ ОК, если метод получает переход, или \_ значение false, если не удается найти переход. В противном случае возвращает значение **HRESULT** , указывающее причину сбоя.

## <a name="remarks"></a>Remarks

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

[**Интерфейс Иамтимелинетрансабле**](iamtimelinetransable.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




