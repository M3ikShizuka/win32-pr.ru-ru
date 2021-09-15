---
description: Изменения, которые монитор используется для закрепленных панелей инструментов в системе с несколькими мониторами.
title: 'Метод Имултимонитордоккингсите:: Сетмонитор'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMultiMonitorDockingSite.SetMonitor
api_type:
- COM
api_location: ''
ms.assetid: ba4ace13-7096-4f05-bcb0-ab37f1632406
ms.openlocfilehash: be773ee68c214f6a2fab8da89f1f48b867e71239
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574551"
---
# <a name="imultimonitordockingsitesetmonitor-method"></a>Метод Имултимонитордоккингсите:: Сетмонитор

Изменения, которые монитор используется для закрепленных панелей инструментов в системе с несколькими мониторами.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT SetMonitor(
  [in]  IUnknown *punkSrc,
  [in]  HMONITOR hMonNew,
  [out] HMONITOR *phMonOld
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пунксрк* \[ окне\]
</dt> <dd>

Тип: **[ **IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown)\***

Указатель на объект, реализующий интерфейс [**идоккингвиндов**](/windows/desktop/api/shobjidl_core/nn-shobjidl_core-idockingwindow) , для которого изменяется монитор.

</dd> <dt>

*хмоннев* \[ окне\]
</dt> <dd>

Тип: **хмонитор**

Маркер монитора, который заменяет существующий монитор по умолчанию.

</dd> <dt>

*фмонолд* \[ заполняет\]
</dt> <dd>

Тип: **хмонитор \***

При возврате этой функции содержит указатель на предыдущий обработчик монитора по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/> |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                   |



 

 
