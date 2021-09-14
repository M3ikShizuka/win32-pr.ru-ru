---
description: Метод Жетдефаултеффект извлекает результат по умолчанию. Если механизм визуализации не может обработать результат, он подставляет результат по умолчанию.
ms.assetid: 27eec6e8-702f-4e56-8d81-aa0633b8ec68
title: 'Метод Иамтимелине:: Жетдефаултеффект (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimeline.GetDefaultEffect
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: a0b1cf356a9c067ccae246814d2e1f381d7f78e5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054578"
---
# <a name="iamtimelinegetdefaulteffect-method"></a>Метод Иамтимелине:: Жетдефаултеффект

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`GetDefaultEffect`Метод получает результат по умолчанию. Если механизм визуализации не может обработать результат, он подставляет результат по умолчанию.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetDefaultEffect(
   GUID *pGuid
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пгуид* 
</dt> <dd>

Получает глобальный уникальный идентификатор (GUID) действия по умолчанию.

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

 

 




