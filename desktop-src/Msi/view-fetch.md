---
description: Метод Fetch объекта View возвращает следующую строку данных столбца, если в результирующем наборе доступно больше строк, в противном случае — значение null. Вызовите метод Execute перед методом FETCH.
ms.assetid: d51bf60d-5725-41eb-9002-1d0e5b9f50a3
title: Метод представления. FETCH
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- View.Fetch
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: b05144b542fd1daa1fc59e12d8ab9ec7031c4a3a5eb6506e9d1316a29b4424ec
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120039494"
---
# <a name="viewfetch-method"></a>Метод представления. FETCH

Метод **Fetch** объекта [**View**](view-object.md) возвращает следующую строку данных столбца, если в результирующем наборе доступно больше строк, в противном случае — значение null. Вызовите метод [**EXECUTE**](view-execute.md) перед методом **Fetch** .

## <a name="syntax"></a>Синтаксис


```JScript
View.Fetch()
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Один и тот же объект [**записи**](record-object.md) следует использовать для получения данных в нескольких строках, иначе объект должен быть освобожден путем выхода из области видимости. Запись можно проверить на конец результирующего набора, используя синтаксис "If Фетчрекорд Nothing".

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ IView определен как 000C109C-0000-0000-C000-000000000046<br/>                                                                                                                                                                                |



 

 




