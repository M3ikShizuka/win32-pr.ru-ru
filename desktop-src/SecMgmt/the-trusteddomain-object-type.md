---
description: системы на основе Windows могут иметь несколько экземпляров типа объекта трустеддомаин.
ms.assetid: 13efedb5-ebb6-459b-8c4f-06774226278c
title: Тип объекта Трустеддомаин
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 70f0a4e6eca0790d877a9a23e4d83725d4e80798
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056962"
---
# <a name="the-trusteddomain-object-type"></a>Тип объекта Трустеддомаин

системы на основе Windows могут иметь несколько экземпляров типа объекта [**трустеддомаин**](trusteddomain-object.md) . Объекты **трустеддомаин** имеют два поля, которые должны быть уникальными для всех объектов **трустеддомаин** :

-   Имя [ **трустеддомаин**](trusteddomain-object.md)
-   [*Идентификатор безопасности*](/windows/desktop/SecGloss/s-gly) (SID) [**трустеддомаин**](trusteddomain-object.md).

Попытка создать новый объект **трустеддомаин** с именем или идентификатором безопасности, который уже используется другим объектом **трустеддомаин** , будет отклонен.

 

 
