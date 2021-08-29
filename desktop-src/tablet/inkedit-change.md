---
description: Происходит при изменении содержимого элемента управления InkEdit.
ms.assetid: 6c65fcca-c84a-414c-a4e5-c5fdffb13e51
title: Событие InkEdit. Change (with. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3679b32b633a9983cc239fdf232491ce13b7805c053c9e1c268c84b9932586ee
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119712974"
---
# <a name="inkeditchange-event"></a>Событие InkEdit. Change

Происходит при изменении содержимого элемента управления [InkEdit](inkedit-control-reference.md) .

## <a name="syntax"></a>Синтаксис


```C++
void Change();
```



## <a name="parameters"></a>Параметры

У этого события нет параметров.

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Это событие возникает при каждом изменении любого свойства, влияющего на содержимое элемента управления [InkEdit](inkedit-control-reference.md) .

Этот метод события определен в интерфейсе **\_ иинкедитевентс** . Интерфейс **\_ иинкедитевентс** реализует интерфейс IDispatch с идентификатором **DISPID \_ иичанже**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>«С». h (также требует \_ ввода i. c)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>InkEd.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[InkEdit](inkedit-control-reference.md)
</dt> </dl>

 

 




