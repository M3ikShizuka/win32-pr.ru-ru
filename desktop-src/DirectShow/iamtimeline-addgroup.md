---
description: Метод AddGroup добавляет группу на временную шкалу.
ms.assetid: c7fc3b59-5852-4a3c-b9bf-f87e659819b5
title: 'Метод Иамтимелине:: AddGroup (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimeline.AddGroup
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: f9557b7937bc0426d0d0c2d8efc24ada968d047460c2d7b3c2f8b1c4c3abccff
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119330294"
---
# <a name="iamtimelineaddgroup-method"></a>Метод Иамтимелине:: AddGroup

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`AddGroup`Метод добавляет группу на временную шкалу.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT AddGroup(
   IAMTimelineObj *pGroup
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пграуп* 
</dt> <dd>

Указатель на интерфейс [**иамтимелинеобж**](iamtimelineobj.md) группы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из следующих значений **HRESULT** :



| Код возврата                                                                                   | Описание                                   |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>          | Успешно.<br/>                           |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl>  | Превышено максимальное число групп.<br/> |
| <dl> <dt>**\_интерфейс E**</dt> </dl> | Объект не является группой.<br/>         |



 

## <a name="remarks"></a>Remarks

Сейчас шкала времени поддерживает не более 32 групп.

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Requirements (Требования)



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

 

 




