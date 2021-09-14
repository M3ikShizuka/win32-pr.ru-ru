---
description: 'Метод Сетсубобжектгуидб указывает идентификатор GUID для подобъекта, связанного с этим объектом. Этот метод эквивалентен Иамтимелинеобж:: Сетсубобжектгуид, но принимает значение BSTR.'
ms.assetid: b2523b17-1df3-4be5-8bbb-6b67815f9349
title: 'Метод Иамтимелинеобж:: Сетсубобжектгуидб (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineObj.SetSubObjectGUIDB
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 8df74249f061321ccd710822b8c2e0b76d5c3582
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053888"
---
# <a name="iamtimelineobjsetsubobjectguidb-method"></a>Метод Иамтимелинеобж:: Сетсубобжектгуидб

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetSubObjectGUIDB`Метод указывает идентификатор GUID подобъекта, связанного с этим объектом. Этот метод эквивалентен [**иамтимелинеобж:: сетсубобжектгуид**](iamtimelineobj-setsubobjectguid.md) , но принимает значение **BSTR** .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetSubObjectGUIDB(
   BSTR newVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*неввал* 
</dt> <dd>

**BSTR** , представляющий идентификатор GUID подобъекта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает \_ значение ОК в случае успешного выполнения или **HRESULT** , указывающий на причину ошибки.

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

[**Интерфейс Иамтимелинеобж**](iamtimelineobj.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




