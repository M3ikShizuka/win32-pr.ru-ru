---
description: Действие RegisterUser регистрирует сведения о пользователе с помощью установщика для обнаружения пользователя продукта.
ms.assetid: da615cb4-d36d-4180-8f97-c9f83c0df1c6
title: Действие RegisterUser
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 686628d29094f951994b072ad4451a383a405965
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057638"
---
# <a name="registeruser-action"></a>Действие RegisterUser

Действие RegisterUser регистрирует сведения о пользователе с помощью установщика для обнаружения пользователя продукта.

## <a name="sequence-restrictions"></a>Ограничения последовательности

Ограничения последовательности отсутствуют.

## <a name="actiondata-messages"></a>Сообщения Актиондата



| Поле | Описание данных действия   |
|-------|------------------------------|
| \[1\] | Зарегистрированные сведения о пользователе. |



 

## <a name="remarks"></a>Комментарии

Действие RegisterUser не выполняется во время административной установки. Если идентификатор продукта, введенный пользователем, не был проверен [действием валидатепродуктид](validateproductid-action.md), свойство [**ProductID**](productid.md) не задается и это действие не выполняет никаких действий.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**ИМЕН**](username.md)
</dt> <dt>

[**Название**](companyname.md)
</dt> <dt>

[**Кодом**](productid.md)
</dt> </dl>

 

 



