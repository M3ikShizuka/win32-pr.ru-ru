---
description: интерфейс иамтимелинесплиттабле разделяет объект timeline в службах DirectShow editing Services (DES). Этот интерфейс реализуется источниками, эффектами, переходами и дорожками.
ms.assetid: bb066d34-0ffd-495f-83ce-59ad054a7782
title: Интерфейс Иамтимелинесплиттабле (Кедит. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineSplittable
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 7b9544809068029b4ca583e83831f9b18ac84e44
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053879"
---
# <a name="iamtimelinesplittable-interface"></a>Интерфейс Иамтимелинесплиттабле

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`IAMTimelineSplittable`интерфейс разделяет объект временной шкалы в [DirectShow службы редактирования](directshow-editing-services.md) (DES). Этот интерфейс реализуется источниками, эффектами, переходами и дорожками.

## <a name="members"></a>Элементы

Интерфейс **иамтимелинесплиттабле** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **Иамтимелинесплиттабле** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **иамтимелинесплиттабле** содержит следующие методы.



| Метод                                             | Описание                                                                                          |
|:---------------------------------------------------|:-----------------------------------------------------------------------------------------------------|
| [**сплитат**](iamtimelinesplittable-splitat.md)   | Разделяет объект в указанное время.<br/>                                                  |
| [**SplitAt2**](iamtimelinesplittable-splitat2.md) | Разделяет объект в указанное время, заданное как значение [**рефтиме**](reftime.md) .<br/> |



 

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



 

 
