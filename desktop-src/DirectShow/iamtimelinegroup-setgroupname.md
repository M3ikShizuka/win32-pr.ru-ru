---
description: Метод Сетграупнаме задает определяемое приложением имя группы.
ms.assetid: e1d8a91b-d5b9-42a4-9b98-582e1a57ac51
title: 'Метод Иамтимелинеграуп:: Сетграупнаме (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineGroup.SetGroupName
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: cf9b80c74c85b335770b6ae0e922d7cc24246b88ab8e7fb7e2b74c396b927a1f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119965124"
---
# <a name="iamtimelinegroupsetgroupname-method"></a>Метод Иамтимелинеграуп:: Сетграупнаме

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetGroupName`Метод задает определяемое приложением имя группы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetGroupName(
   BSTR pGroupName
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пграупнаме* 
</dt> <dd>

**BSTR** , указывающий имя группы. Максимальная длина имени — 256 символов, инкудинг терминатор null.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

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

[**Интерфейс Иамтимелинеграуп**](iamtimelinegroup.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




