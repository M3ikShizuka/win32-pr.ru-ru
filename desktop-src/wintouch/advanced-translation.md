---
title: Расширенный перевод
description: Расширенный перевод
ms.assetid: 48a1bdd5-8b7b-4460-9b7b-1ab8969a28f8
keywords:
- Windows Сенсорный ввод, перевод
- Windows Сенсорный ввод, расширенный перевод
- Windows Сенсорный ввод, манипуляции
- манипуляции, перевод
- манипуляции, расширенный перевод
- преобразование
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bc383c71e1f1417d30b64db18aa627039602b942
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127251593"
---
# <a name="advanced-translation"></a>Расширенный перевод

На следующем рисунке показаны две интерпретации преобразования.

![Иллюстрация, на которой сначала показан простой перевод, в котором объект перемещается без вращения, а затем отображается расширенный перевод, включающий перемещение с поворотом.](images/translation.png)

В примере с простым примером перевода объект перемещается без вращения. В примере б объект поворачивается во время перевода, в зависимости от того, где находится точка контакта объекта. При включении ротации с одним пальцем, как описано в разделе [однонаправленный поворот](single-finger-rotation.md), можно включить сложный перевод. На следующей диаграмме показаны различные компоненты ротации с одним пальцем при выполнении перевода.

![Иллюстрация, в которой показаны компоненты ротации с одним пальцем: пивотпоинткс, пивотпоинти и пивотрадиус](images/translation-complex-components.png)

При перемещении объекта происходит повторное вычисление радиуса и перемещение точки вращения.

В следующем коде показан один из способов, которые можно выполнить в реализации [**ManipulationDelta**](/windows/win32/api/manipulations/nf-manipulations-_imanipulationevents-manipulationdelta) , которая обеспечивает сложный перевод.


```C++
    //Apply transformation based on rotationDelta (in radians)
    FLOAT rads = 180.0f / 3.14159f;
    m_dObj->Rotate(rotationDelta*rads, x, y);

    // Apply translation based on scaleDelta
    m_dObj->Scale(scaleDelta);

    // Apply translation based on translationDelta
    m_dObj->Translate(translationDeltaX, translationDeltaY);

    // Set values for one finger rotations
    FLOAT fPivotRadius = (FLOAT)(m_dObj->get_Width() + m_dObj->get_Height())/8.0f;
    FLOAT fPivotPtX = m_dObj->get_CenterX();
    FLOAT fPivotPtY = m_dObj->get_CenterY();
        
    m_manip->put_PivotPointX(fPivotPtX);
    m_manip->put_PivotPointY(fPivotPtY);
    m_manip->put_PivotRadius(fPivotRadius);       
   
```



> [!Note]  
> Преобразования объектов происходят до вычисления точек вращения и RADIUS. Таким образом объект будет перемещаться правильно, если пользователь выполняет расширение объекта во время его перемещения.

 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Манипуляции](getting-started-with-manipulations.md)
</dt> </dl>

 

 




