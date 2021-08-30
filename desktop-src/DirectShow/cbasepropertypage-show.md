---
description: 'Метод «Показать» показывает или скрывает диалоговое окно. Этот метод реализует метод Ипропертипаже:: демонстрации.'
ms.assetid: 03796779-ed41-4b68-852d-6b1849a9dc10
title: Метод Кбасепропертипаже. показывать (Кпроп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBasePropertyPage.Show
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4a05a04e1012824e1204318fc3bddaf3e0317c32f3e53fa0e6a5a46f7dd1b50a
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120103194"
---
# <a name="cbasepropertypageshow-method"></a>Кбасепропертипаже. отобразить метод

`Show`Метод показывает или скрывает диалоговое окно. Этот метод реализует метод [ипропертипаже:: демонстрации](/windows/win32/api/ocidl/nf-ocidl-ipropertypage-show) .

## <a name="syntax"></a>Синтаксис

```C++
HRESULT Show(
   UINT nCmdShow
);
```
## <a name="parameters"></a>Параметры

*нкмдшов*

Тип: **[uint](../winprog/windows-data-types.md)**

Значение, указывающее, следует ли отображать или скрывать окно. Дополнительные сведения см. в описании метода [ипропертипаже:: Показать](/windows/win32/api/ocidl/nf-ocidl-ipropertypage-show) .

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Ниже приведены возможные значения.

| Код возврата                                                                                  | Описание                    |
|----------------------------------------------------------------------------------------------|--------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Успешно.<br/>            |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Недопустимый аргумент.<br/>   |
| <dl> <dt>**\_непредвиденная E**</dt> </dl> | Непредвиденный сбой.<br/> |

## <a name="requirements"></a>Requirements (Требования)

| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок  | <dl> <dt>кпроп. h (включает Потоки. h)</dt> </dl>                                                                                     |
| Библиотека | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |

## <a name="see-also"></a>См. также

[Класс Кбасепропертипаже](cbasepropertypage.md)
