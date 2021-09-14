---
description: Метод Жетаутпутфпс извлекает частоту кадров вывода для этой группы.
ms.assetid: e6dfa4a9-4d44-4ce7-9aec-3564fd337ff6
title: 'Метод Иамтимелинеграуп:: Жетаутпутфпс (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineGroup.GetOutputFPS
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 2f02e7db36e5ea61e3c738b4c2d92678674bfcec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126887000"
---
# <a name="iamtimelinegroupgetoutputfps-method"></a>Метод Иамтимелинеграуп:: Жетаутпутфпс

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`GetOutputFPS`Метод извлекает частоту выходных кадров этой группы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetOutputFPS(
   double *pFPS
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пфпс* 
</dt> <dd>

Получает частоту кадров вывода в кадрах в секунду.

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

[**Интерфейс Иамтимелинеграуп**](iamtimelinegroup.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




