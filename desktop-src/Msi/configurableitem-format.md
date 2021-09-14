---
description: Свойство Format объекта Конфигураблеитем возвращает значение из столбца Format таблицы Модулеконфигуратион.
ms.assetid: e75ed650-7309-4e24-9c35-82ebf27d011b
title: Свойство Конфигураблеитем. Format (Мержемод. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ConfigurableItem.Format
- IMsmConfigurableItem.get_Format
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: 20db09126e9b10aac5c31a3748c4f1606f3f3bab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127142270"
---
# <a name="configurableitemformat-property"></a>Конфигураблеитем. Format, свойство

Свойство **Format** объекта [**конфигураблеитем**](configurableitem-object.md) возвращает значение из столбца Format [таблицы модулеконфигуратион](moduleconfiguration-table.md).

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = ConfigurableItem.Format
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Это свойство может иметь только следующие значения.



| Константа                        | Значение |
|---------------------------------|-------|
| **мсмконфигураблеитемтекст**     | 0     |
| **мсмконфигураблеитемкэй**      | 1     |
| **мсмконфигураблеитеминтежер**  | 2     |
| **мсмконфигураблеитембитфиелд** | 3     |



 

### <a name="c"></a>C++

См. раздел [**Получение функции \_ форматирования**](/windows/desktop/api/Mergemod/nf-mergemod-imsmconfigurableitem-get_format) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 2,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

 




