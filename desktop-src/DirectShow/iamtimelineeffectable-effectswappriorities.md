---
description: Метод Еффектсвапприоритиес переключает уровни приоритета двух эффектов.
ms.assetid: ff5ab294-3963-4df7-9299-ee7c7165e72f
title: 'Метод Иамтимелиниффектабле:: Еффектсвапприоритиес (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineEffectable.EffectSwapPriorities
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: fb6a7dbee2d7f90da8f32e2a034e82df485f1ef4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126887053"
---
# <a name="iamtimelineeffectableeffectswappriorities-method"></a>Метод Иамтимелиниффектабле:: Еффектсвапприоритиес

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`EffectSwapPriorities`Метод переключает уровни приоритета двух эффектов.

При наличии двух значений приоритета этот метод меняет местами эти приоритеты. При возврате из метода результат, который был на первом уровне приоритета, находится на втором уровне приоритета, и наоборот.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT EffectSwapPriorities(
   long PriorityA,
   long PriorityB
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Приоритет* 
</dt> <dd>

Первый уровень приоритета для переключения эффектов.

</dd> <dt>

*приоритиб* 
</dt> <dd>

Второй уровень приоритета для переключения эффектов.

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

[**Интерфейс Иамтимелиниффектабле**](iamtimelineeffectable.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




