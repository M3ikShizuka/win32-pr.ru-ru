---
description: Метод Жетсубобжект извлекает подобъект, связанный с этим объектом.
ms.assetid: 478597d6-ae13-4fa9-a928-19893f378f1a
title: 'Метод Иамтимелинеобж:: Жетсубобжект (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineObj.GetSubObject
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 74f14658db5ffbaf100925f26573a08b592f6510
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126886949"
---
# <a name="iamtimelineobjgetsubobject-method"></a>Метод Иамтимелинеобж:: Жетсубобжект

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`GetSubObject`Метод извлекает подобъект, связанный с этим объектом.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetSubObject(
  [out, retval] IUnknown **pVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Pval* \[ out, retval\]
</dt> <dd>

Получает указатель на интерфейс **IUnknown** подобъекта. Если у объекта нет подобъекта, ему присваивается значение **null**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Каждый объект временной шкалы может содержать указатель на связанный с ним подобъект.

Если значение, возвращаемое в *Pval* , не равно **null**, то интерфейс **IUnknown** имеет необработанный счетчик ссылок. Не забудьте освободить интерфейс по завершении его использования.

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

 

 




