---
description: вы можете установить все продукты с помощью функций установщик Windows. Ниже описана процедура установки продукта.
ms.assetid: 03cc7abc-63bd-4a01-a05c-9f7928de8827
title: Установка приложения
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 74aad6e130d78bd30b940232aeb6fe1da6508be754fe50b9abb9dbcaa0186562
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119327964"
---
# <a name="installing-an-application"></a>Установка приложения

вы можете установить все продукты с помощью функций установщик Windows. Ниже описана процедура установки продукта.

**Установка продукта**

1.  Запустите продукт через его установку или последовательность удаления, вызвав функцию [**мсиинсталлпродукт**](/windows/desktop/api/Msi/nf-msi-msiinstallproducta) .
2.  Укажите уровень установки, вызвав функцию [**мсиконфигурепродукт**](/windows/desktop/api/Msi/nf-msi-msiconfigureproducta) .

    Для установки состояния установки можно использовать параметры функции [**мсиконфигурепродукт**](/windows/desktop/api/Msi/nf-msi-msiconfigureproducta) . Например, можно задать для состояния значение установить локально или установить из источника. Вы можете задать диапазон компонентов продукта, который будет включен, задав уровень.

Дополнительные сведения об установке приложения см. в разделе механизм [устойчивости](resiliency.md) и [установки](installation-mechanism.md).

 

 



