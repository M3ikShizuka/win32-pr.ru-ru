---
title: Call-PS
description: Выполняет вызов функции в инструкцию, помеченную указанной меткой. | Call-PS
ms.assetid: d5f5e5a1-f205-477d-a11b-ff9eeeec6c95
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- apiref
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 27be29c478afdf92c29fefd16a82319e0899d2ec
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574014"
---
# <a name="call---ps"></a>Call-PS

Выполняет вызов функции в инструкцию, помеченную указанной меткой.

## <a name="syntax"></a>Синтаксис



| вызов l\# |
|----------|



 

Где:

-   l \# — [Метка-PS](label---ps.md) , помечающая начало подпрограммы для вызова.

## <a name="remarks"></a>Комментарии



| Версии шейдеров пикселей | 1\_1 | 1\_2 | 1 \_ 3 | 1\_4 | 2 \_ 0 | 2 \_ x | 2 \_ SW | 3 \_ 0 | 3 \_ SW |
|-----------------------|------|------|------|------|------|------|-------|------|-------|
| вызывает                  |      |      |      |      |      | x    | x     | x    | x     |



 

Эта инструкция выполняет следующие действия:

1.  Адрес принудительной отправки следующей инструкции в стек адресов возврата.
2.  Продолжить выполнение из инструкции, помеченной меткой.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Инструкции шейдера пикселей](dx9-graphics-reference-asm-ps-instructions.md)
</dt> </dl>

 

 




