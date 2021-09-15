---
title: Метка — VS
description: Пометьте следующую инструкцию как индекс метки. | Метка — VS
ms.assetid: e1aee8bc-4655-4bd5-8012-bd7a2d46e712
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 6e2b72fe21301aa66d8428dc3696ceb3f12e6214
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567759"
---
# <a name="label---vs"></a>Метка — VS

Пометьте следующую инструкцию как индекс метки.

## <a name="syntax"></a>Синтаксис



| Метка l\# |
|-----------|



 

где \# определяет номер метки.

Для VS \_ 2 \_ 0 и VS \_ 2 \_ x номер метки должен находиться в диапазоне от 0 до 15.

Для VS \_ 2 \_ SW, VS \_ 3 \_ 0 и VS \_ 3 \_ SW номер метки должен находиться в диапазоне от 0 до 2047.

## <a name="remarks"></a>Комментарии



| Версии шейдеров вершин | 1\_1 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|------------------------|------|------|------|-------|------|-------|
| label                  |      | x    | x    | x     | x    | x     |



 

Эта инструкция определяет метку, расположенную в следующей инструкции шейдера. Инструкция Label может присутствовать непосредственно после инструкции [RET](ret---vs.md) (которая определяет конец предыдущей подпрограммы или основной программы).

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Инструкции шейдера вершин](dx9-graphics-reference-asm-vs-instructions.md)
</dt> </dl>

 

 




