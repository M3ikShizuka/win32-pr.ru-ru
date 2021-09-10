---
title: Оператор разрешения области в C++
description: Оператор разрешения области в C++
ms.assetid: 908cf2b0-41d2-442d-aba8-82f3328c72c1
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: cb888fa9d56b6a84f8ecbc5efb2c235d1a38be03
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124372486"
---
# <a name="the-scope-resolution-operator-in-c"></a>Оператор разрешения области в C++

Два двоеточия (::) используются в C++ в качестве оператора *разрешения области* . Этот оператор обеспечивает большую свободу при именовании переменных, позволяя различать переменные с одинаковыми именами. Например, класс *MyFile:: Read* относится к методу *Read* класса *MyFile* объектов, а не к *йоурфиле:: Read*, который ссылается на метод *Read* в классе *йоурфиле* .

 

 




