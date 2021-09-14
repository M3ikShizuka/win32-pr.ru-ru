---
title: Эффекты оттенков серого
description: Преобразовывает изображение с использованием монохромных серых оттенков.
ms.assetid: 4e0b26ed-ba71-5f8f-db1e-f1b4e28fbd11
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e0dc3cb6a807d282649a2826713cdf48fa966d9f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163247"
---
# <a name="grayscale-effect"></a>Эффекты оттенков серого

Преобразовывает изображение с использованием монохромных серых оттенков.

В градациях серого используется Цветовая матрица для преобразования в градации серого с использованием следующей матрицы:

![Матрица преобразования](images/grayscale-effect-matrix.png)

Идентификатором CLSID для этого действия является CLSID \_ D2D1Grayscale.

-   [Пример изображения](#example-image)
-   [Свойства эффектов](#effect-properties)
-   [Requirements](#requirements)
-   [Связанные темы](#related-topics)

## <a name="example-image"></a>Пример изображения

![Пример выходных данных эффектов](images/grayscale-effect.png)

## <a name="effect-properties"></a>Свойства эффектов

У этого действия нет свойств.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------------|---------------------------------------------------|
| Минимальная версия клиента | Windows 10 \[ классические приложения \| Windows приложения магазина\] |
| Минимальная версия сервера | Windows 10 \[ классические приложения \| Windows приложения магазина\] |
| Заголовок                   | d2d1effects \_ 2. h                                  |
| Библиотека                  | D2D1. lib, дксгуид. lib                              |


## <a name="related-topics"></a>Связанные темы

* [Интерфейс ID2D1Effect](/windows/desktop/api/d2d1_1/nn-d2d1_1-id2d1effect)
