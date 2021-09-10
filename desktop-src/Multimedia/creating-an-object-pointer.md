---
title: Создание указателя на объект
description: Создание указателя на объект
ms.assetid: b66a2725-6ba1-4aea-b165-fe3f4da00375
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4f57451e2781a94642e61365d3a6c694758f4056
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371673"
---
# <a name="creating-an-object-pointer"></a>Создание указателя на объект

Авибалл использует в качестве указателя на объект следующую структуру. Первый элемент этой структуры указывает на таблицу виртуальной функции, которую Авибалл использует для доступа к ее функциям. Приложения могут привести эту структуру к типу данных ПАВИСТРЕАМ. Методы, использующие тип данных ПАВИСТРЕАМ, используют только указатель на таблицу виртуальной функции. Элементы, следующие за указателем на таблицу виртуальной функции, используются внутренне Авибалл.


```C++
typedef struct 
{ 
    IAVIStreamVtbl FAR * lpvtbl; 
 
    // Ball instance data. 
    ULONG     ulRefCount; 
    DWORD     fccType;  // is this audio/video? 
    int        width;    // size, in pixels, of each frame 
    int        height; 
    int        length;   // length, in frames 
    int        size; 
    COLORREF    color;    // ball color 
} AVIBALL, FAR * PAVIBALL; 

```



 

 




