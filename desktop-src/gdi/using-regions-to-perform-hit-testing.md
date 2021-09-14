---
description: В примере кистей используются регионы для имитации &\# 0034; с масштабированием&\# 0034; представление растрового изображения размером 8 в 8 пикселей.
ms.assetid: a8e0cbfe-f05b-46ae-b420-ae34a5efbff3
title: Использование регионов для проверки попадания
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bb50ca1f837213b85619af381b86c2bd76efcbb9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462270"
---
# <a name="using-regions-to-perform-hit-testing"></a>Использование регионов для проверки попадания

В примере в [кистях](brushes.md) используются регионы для имитации "масштабированного" изображения с монохромным изображением размером 8 пикселей. Щелкая Пиксели в этом битовом рисунке, пользователь создает пользовательскую кисть, подходящую для операций рисования. В примере показано, как использовать функцию [**птинрегион**](/windows/desktop/api/Wingdi/nf-wingdi-ptinregion) для проверки попадания и функции [**инвертргн**](/windows/desktop/api/Wingdi/nf-wingdi-invertrgn) для инвертирования цветов в области.

 

 



