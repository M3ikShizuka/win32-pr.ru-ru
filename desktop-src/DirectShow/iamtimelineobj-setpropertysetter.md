---
description: Метод Сетпропертисеттер устанавливает метод задания свойства объекта. При подготовке к просмотру объекта сведения о свойствах, содержащиеся в методе задания свойств, применяются к объекту. Вызывайте этот метод для объектов перехода и эффектов.
ms.assetid: 3ce2fe50-a884-4da4-95b5-9c97e188f819
title: 'Метод Иамтимелинеобж:: Сетпропертисеттер (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineObj.SetPropertySetter
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: c347296221cae30063a9d1e775252654df6b8daf592b2321b68d35067751ad15
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119213574"
---
# <a name="iamtimelineobjsetpropertysetter-method"></a>Метод Иамтимелинеобж:: Сетпропертисеттер

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`SetPropertySetter`Метод задает свойство метода для свойства объекта. При подготовке к просмотру объекта сведения о свойствах, содержащиеся в методе задания свойств, применяются к объекту. Вызывайте этот метод для объектов перехода и эффектов.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetPropertySetter(
   IPropertySetter *newVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*неввал* 
</dt> <dd>

Указатель на интерфейс [**ипропертисеттер**](ipropertysetter.md) метода задания свойств.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

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

[**Интерфейс Иамтимелинеобж**](iamtimelineobj.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




