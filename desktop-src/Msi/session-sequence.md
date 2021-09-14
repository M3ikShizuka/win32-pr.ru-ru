---
description: Метод Sequence объекта Session открывает запрос к указанной таблице, упорядочивая действия по числам в столбце последовательности.
ms.assetid: cde735b0-0b97-4c4f-adfc-f0321aafb012
title: Session. Sequence, метод
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Session.Sequence
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 18708b79bdce73b29f46b4d62a15ceb8003d9c9b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272464"
---
# <a name="sessionsequence-method"></a>Session. Sequence, метод

Метод **Sequence** объекта [**Session**](session-object.md) открывает запрос к указанной таблице, упорядочивая действия по числам в столбце последовательности. Для каждой выбранной строки вызывается метод [**DoAction**](session-doaction.md) при условии, что любое предоставленное выражение условия не возвращает значение false. Возвращает Мсидоактионстатусенум перечисления, как описано в методе [**DoAction**](session-doaction.md) .

## <a name="syntax"></a>Синтаксис


```JScript
Session.Sequence(
  table
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*table* 
</dt> <dd>

Обязательное строковое имя таблицы, используемой для виртуализации.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод обычно вызывается внутренним действием верхнего уровня.

Последовательность действий, содержащая действия, которые обновляют систему, такие как действия [инсталлфилес](installfiles-action.md) и [вритерегистривалуес](writeregistryvalues-action.md) , не может быть выполнена путем вызова метода **Sequence** . Исключением из этого правила является то, что метод **Sequence** вызывается из настраиваемого действия, запланированного в [таблице инсталлексекутесекуенце](installexecutesequence-table.md) между [действиями](installfinalize-action.md) [инсталлинитиализе](installinitialize-action.md) и функции InstallFinalize. Действия, которые не обновляют систему, например [аппсеарч](appsearch-action.md) или [костинитиализе](costinitialize-action.md), могут быть вызваны.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ISession определяется как 000C109E-0000-0000-C000-000000000046<br/>                                                                                                                                                                             |



 

 




