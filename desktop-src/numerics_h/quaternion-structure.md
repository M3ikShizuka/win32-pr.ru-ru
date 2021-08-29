---
title: Структура кватерниона (Виндовснумерикс. h)
description: 4-мерный вектор, используемый для представления вращения.
ms.assetid: A6B25885-8ECB-4039-9DC6-41D5F3A02489
keywords:
- Структура кватерниона
topic_type:
- apiref
api_name:
- quaternion structure
api_location:
- windowsnumerics.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 16688687b494fac98074ce933ba01dc194093da0ed2013b51f0bee0f41f31b3f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119825224"
---
# <a name="quaternion-structure"></a>Структура кватерниона

4-мерный вектор, используемый для представления вращения.

Кватернион может эффективно поворачивать объект вокруг вектора (x, y, z) на угол тета, где w = cos (тета/2). Кватернионы обычно используются для плавной интерполяции между двумя углами и для предотвращения проблемы с блокировкой гимбал, которая может возникнуть с Эйлера углами.

Этот тип доступен только в C++. Его эквивалент .NET — [System. Numerics. кватернион](/dotnet/api/system.numerics.quaternion?view=netframework-4.8).

## <a name="constructors"></a>Конструкторы

| Имя | Описание |
|-|-|
| `quaternion()` | Создает неинициализированный кватернион. |
| `quaternion(float x, float y, float z, float w)` | Создает кватернион с указанными значениями. |
| `quaternion(float3 vectorPart, float scalarPart)` | Создает кватернион из float3 и скалярного. |
| `quaternion(Microsoft::?Graphics::?Canvas::?Numerics::?Quaternion const& value)` | Преобразует объект **Microsoft. Graphics. Холст. Numerics. кватернион** в кватернион. |

## <a name="functions"></a>Функции

| Имя | Описание |
|-|-|
| `quaternion make_quaternion_from_axis_angle(float3 const& axis, float angle)` | Создает кватернион на основе вектора и угла поворота вокруг вектора. |
| `quaternion make_quaternion_from_yaw_pitch_roll(float yaw, float pitch, float roll)` | Создает кватернион на основе указанных значения нутации, высоты и углов. |
| `quaternion make_quaternion_from_rotation_matrix(float4x4 const& matrix)` | Создает кватернион из матрицы вращения. |
| `bool is_identity(quaternion const& value)` | Проверяет, является ли этот кватернион единичным (без поворота). |
| `float length(quaternion const& value)` | Вычисляет длину кватерниона. |
| `float length_squared(quaternion const& value)` | Вычисляет длину объекта Quaternion в квадрате. |
| `float dot(quaternion const& quaternion1, quaternion const& quaternion2)` | Вычисляет скалярное произведение двух кватернионов. |
| `quaternion normalize(quaternion const& value)` | Делит каждый компонент кватерниона на длину кватерниона. |
| `quaternion conjugate(quaternion const& value)` | Вычисляет сопряженный кватернион. |
| `quaternion inverse(quaternion const& value)` | Вычисляет обратную часть кватерниона. |
| `quaternion slerp(quaternion const& quaternion1, quaternion const& quaternion2, float amount)` | Выполняет интерполяцию между двумя кватернионами, используя сферическую линейную интерполяцию. |
| `quaternion lerp(quaternion const& quaternion1, quaternion const& quaternion2, float amount)` | Линейная интерполяция между двумя кватерниона. |
| `quaternion concatenate(quaternion const& value1, quaternion const& value2)` | Сцепляет два кватерниона; Результат представляет первый поворот, за которым следует второй поворот. |

## <a name="methods"></a>Методы

| Имя | Описание |
|-|-|
| `static quaternion identity()` | Возвращает экземпляр идентификатора кватерниона. |

## <a name="operators"></a>Операторы

| Имя | Описание |
|-|-|
| `quaternion operator+ (quaternion const& value1, quaternion const& value2)` | Складывает два кватерниона. |
| `quaternion operator- (quaternion const& value1, quaternion const& value2)` | Вычитает кватернион из другого кватерниона. |
| `quaternion operator* (quaternion const& value1, quaternion const& value2)` | Умножает кватернион на другой кватернион. |
| `quaternion operator* (quaternion const& value1, float value2)` | Умножает кватернион на скалярное значение. |
| `quaternion operator/ (quaternion const& value1, quaternion const& value2)` | Делит кватернион на другой кватернион. |
| `quaternion operator- (quaternion const& value)` | Переворачивает знак каждого компонента кватерниона. |
| `quaternion& operator+= (quaternion& value1, quaternion const& value2)` | На месте добавляется два кватерниона. |
| `quaternion& operator-= (quaternion& value1, quaternion const& value2)` | На месте вычитается кватернион из другого кватерниона. |
| `quaternion& operator*= (quaternion& value1, quaternion const& value2)` | На месте умножает кватернион на другой кватернион. |
| `quaternion& operator*= (quaternion& value1, float value2)` | На месте нултиплиес кватернион скалярным значением. |
| `quaternion& operator/= (quaternion& value1, quaternion const& value2)` | На месте делит кватернион на другой кватернион. |
| `bool operator== (quaternion const& value1, quaternion const& value2)` | Определяет, равны ли два экземпляра кватерниона. |
| `bool operator!= (quaternion const& value1, quaternion const& value2)` | Определяет, являются ли два экземпляра кватерниона неравными. |
| `operator Microsoft::?Graphics::?Canvas::?Numerics::?Quaternion() const` | Преобразует кватернион в объект **Microsoft. Graphics. Холст. Numerics. кватернион**. |

## <a name="fields"></a>Поля

| Имя | Описание |
|-|-|
| `float x` | Значение X компонента вектора кватерниона. |
| `float y` | Значение Y компонента вектора кватерниона. |
| `float z` | Значение Z компонента вектора кватерниона. |
| `float w` | Компонент вращения кватерниона. |

## <a name="requirements"></a>Требования

| Требование | Значение |
|-|-|
| Пространство имен | Windows:: Foundation:: numerics |
| Заголовок | <dl> <dt>Виндовснумерикс. h</dt> </dl> |

## <a name="see-also"></a>См. также раздел

[API-интерфейсы виндовснумерикс. h](windowsnumerics-h-apis-portal.md)
