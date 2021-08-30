---
description: интерфейс иамтимелиневиртуалтракк предоставляет методы для работы с виртуальными дорожками в службах DirectShow editing Services (DES). Этот интерфейс поддерживается композициями и дорожками.
ms.assetid: 69d1d2ea-d33f-406d-a9ca-ddfb890bed34
title: Интерфейс Иамтимелиневиртуалтракк (Кедит. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineVirtualTrack
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: f9eba273793e97c5fb92fdabb365eb2402fc6feb6fbc571f1ec1ef1a0a4b3692
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119982774"
---
# <a name="iamtimelinevirtualtrack-interface"></a>Интерфейс Иамтимелиневиртуалтракк

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`IAMTimelineVirtualTrack`интерфейс предоставляет методы для работы с виртуальными дорожками в [службах DirectShow editing Services](directshow-editing-services.md) (DES). Этот интерфейс поддерживается композициями и дорожками.

## <a name="members"></a>Элементы

Интерфейс **иамтимелиневиртуалтракк** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **Иамтимелиневиртуалтракк** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **иамтимелиневиртуалтракк** содержит следующие методы.



| Метод                                                               | Описание                                       |
|:---------------------------------------------------------------------|:--------------------------------------------------|
| [**сеттраккдирти**](iamtimelinevirtualtrack-settrackdirty.md)       | Не поддерживается.<br/>                         |
| [**траккжетприорити**](iamtimelinevirtualtrack-trackgetpriority.md) | Возвращает уровень приоритета объекта.<br/> |



 

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



 

 
