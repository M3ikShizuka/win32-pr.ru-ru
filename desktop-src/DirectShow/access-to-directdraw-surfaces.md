---
description: Доступ к областям DirectDraw
ms.assetid: 21002c9f-8b8b-49f3-9ea3-3703780e3412
title: Доступ к областям DirectDraw
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ff443550cb6a922a3361b6d75b880eb427edf79e3a3232c21ab6aad0c06ec483
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119873574"
---
# <a name="access-to-directdraw-surfaces"></a>Доступ к областям DirectDraw

Образцы объектов мультимедиа, предоставляемые VMR для вышестоящего фильтра, поддерживают интерфейс [**ивмрсурфаце**](/windows/desktop/api/Strmif/nn-strmif-ivmrsurface) . Чтобы получить интерфейс, вызовите QueryInterface в интерфейсе [**имедиасампле**](/windows/desktop/api/Strmif/nn-strmif-imediasample) и укажите IID \_ ивмрсурфаце. Вышестоящий фильтр может использовать методы Ивмрсурфаце для доступа к поверхности, созданной с помощью VMR, и управления ей.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[использование VMR для разработчиков фильтров DirectShow](using-the-vmr-for-directshow-filter-developers.md)
</dt> </dl>

 

 



