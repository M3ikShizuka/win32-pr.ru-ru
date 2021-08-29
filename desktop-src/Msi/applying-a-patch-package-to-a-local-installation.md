---
description: Вы можете применить небольшое обновление к локальной установке MNP2000 с примером исправления Мнппатч. MSP, созданным при формировании пакета исправлений.
ms.assetid: 928182ae-5ddb-446f-a9b8-e8b3aa4ce49c
title: Применение пакета исправлений к локальной установке
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1db0f29c5ced78ff8f5ad4ce8c667ba7265dd7426f9a34a5d17f743e07bfc6ee
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120078124"
---
# <a name="applying-a-patch-package-to-a-local-installation"></a>Применение пакета исправлений к локальной установке

Вы можете применить небольшое обновление к локальной установке MNP2000 с примером исправления Мнппатч. MSP, созданным при [формировании пакета исправлений](generating-a-patch-package.md). Общая процедура рассматривается в разделе [применение небольших обновлений путем исправления локальной установки продукта](applying-small-updates-by-patching-the-local-installation-of-the-product.md).

Установите исходный продукт MNP2000 локально на компьютере. Убедитесь, что в нем имеется ошибка Concert.txt, что небольшое обновление должно быть исправлено. Затем запустите установку, введя следующую командную строку.

**msiexec/p MNP2000. MSP REINSTALL = ALL REINSTALLMODE = omus**

Повторно проверьте Concert.txt, принадлежащие MNP2000, чтобы убедиться, что установщик установил небольшое обновление для исправления этого файла.

Чтобы применить небольшое обновление к административному образу, см. раздел [Применение пакета исправлений в административной установке](applying-a-patch-package-to-an-administrative-installation.md).

[Продолжить](applying-a-patch-package-to-an-administrative-installation.md)

 

 



