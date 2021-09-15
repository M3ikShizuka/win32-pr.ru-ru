---
title: оптималбитрате
description: Атрибут Оптималбитрате содержит битовую скорость, с которой файл лучше воспроизводить.
ms.assetid: cd13b9b5-34d2-4ebb-9f10-3bf42dd9de81
keywords:
- Формат Windows Media Оптималбитрате
topic_type:
- apiref
api_name:
- OptimalBitrate
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ff71c6b64cbc4bf4ccc4f346e62a5eae066e78ce
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459331"
---
# <a name="optimalbitrate"></a>оптималбитрате

Атрибут **оптималбитрате** содержит битовую скорость, с которой файл лучше воспроизводить.

## <a name="global-constant"></a>Глобальная константа

g \_ всзвмоптималбитрате

## <a name="data-type"></a>Тип данных

**ВМТ, \_ тип \_ DWORD**

## <a name="remarks"></a>Комментарии

Это закодированный атрибут.

Для файлов, содержащих потоки с переменной скоростью (VBR), это значение является пиковой скоростью потока в файле. Для файлов без VBR это значение совпадает с [**скоростью**](bit-rate.md).

Этот атрибут не может дублироваться на уровне файла. если этот атрибут используется для отдельного потока, он будет рассматриваться как пользовательские метаданные и не будет передавать свое нормальное значение объектам из пакета SDK Windows Media Format.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Список атрибутов**](attribute-list.md)
</dt> </dl>

 

 




