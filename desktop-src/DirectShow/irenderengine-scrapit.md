---
description: Метод Скрапит отклоняет граф фильтра механизма отрисовки и все связанные объекты.
ms.assetid: b7470947-a661-4c08-8786-9298e5322e58
title: 'Метод Ирендеренгине:: Скрапит (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IRenderEngine.ScrapIt
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 7f9febbe20cfd5ab9a6577a6e00989c7d6fc4145
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126886720"
---
# <a name="irenderenginescrapit-method"></a>Метод Ирендеренгине:: Скрапит

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`ScrapIt`Метод отклоняет граф фильтра механизма отрисовки и все связанные объекты.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT ScrapIt();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из следующих значений **HRESULT** :



| Код возврата                                                                                            | Описание                                    |
|--------------------------------------------------------------------------------------------------------|------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>                   | Успешно.<br/>                            |
| <dl> <dt>**E \_ должен \_ инициализировать модуль \_ подготовки отчетов**</dt> </dl> | Не удалось инициализировать модуль визуализации.<br/> |



 

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

[**Интерфейс Ирендеренгине**](irenderengine.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




