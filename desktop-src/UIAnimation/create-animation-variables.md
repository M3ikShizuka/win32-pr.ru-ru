---
title: Создание переменных анимации
description: приложение должно создать переменную анимации для каждой визуальной характеристики, которая должна быть анимирована с помощью Windows анимации.
ms.assetid: 360aa157-cb50-400a-b373-45885410469d
keywords:
- переменные анимации Windows анимация, создание
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bb81e2f94f987ad6b9c923083c76565fa75b2cc665753233c8a84b6eb1a1d52a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120008234"
---
# <a name="create-animation-variables"></a>Создание переменных анимации

приложение должно создать переменную анимации для каждой визуальной характеристики, которая должна быть анимирована с помощью Windows анимации.

## <a name="overview"></a>Обзор

Переменные анимации создаются с помощью диспетчера анимации, и приложение должно хранить ссылку на каждый из них, если это необходимо. Приложение, как правило, создает каждую переменную анимации одновременно с визуальным объектом, на котором он анимируется.

При создании переменной анимации необходимо указать ее начальное значение. После этого его значение можно изменить только путем планирования раскадровок, которые ее анимировать.

Переменные анимации передаются как параметры при создании раскадровок, поэтому приложение не должно освобождать их до тех пор, пока визуальные характеристики, которые они представляют, больше не нужны для анимации, как правило, когда связанные визуальные объекты будут уничтожены.

## <a name="example-code"></a>Пример кода

-   [Анимация цветов](#animating-colors)
-   [Анимация координат x и y](#animating-x-and-y-coordinates)

### <a name="animating-colors"></a>Анимация цветов

следующий пример кода взят из файла MainWindow. cpp в Windows анимация, [управляемая приложениями](application-driven-animation-sample.md) , и анимация, [управляемая таймером](timer-driven-animation-sample.md). В этом примере три переменные анимации создаются с помощью [**креатеаниматионвариабле**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationmanager-createanimationvariable) для представления цветов фона. Код также использует методы [**сетловербаунд**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationvariable-setlowerbound) и [**сетуппербаунд**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationvariable-setupperbound) для управления значением переменной анимации.


```
const DOUBLE INITIAL_RED = COLOR_MAX;
const DOUBLE INITIAL_GREEN = COLOR_MAX;
const DOUBLE INITIAL_BLUE = COLOR_MAX;

HRESULT hr = m_pAnimationManager->CreateAnimationVariable(
    INITIAL_RED,
    &m_pAnimationVariableRed
    );
if (SUCCEEDED(hr))
{
    hr = m_pAnimationVariableRed->SetLowerBound(COLOR_MIN);
    if (SUCCEEDED(hr))
    {
        hr = m_pAnimationVariableRed->SetUpperBound(COLOR_MAX);
        if (SUCCEEDED(hr))
        {
            hr = m_pAnimationManager->CreateAnimationVariable(
                INITIAL_GREEN,
                &m_pAnimationVariableGreen
                );
            if (SUCCEEDED(hr))
            {
                hr = m_pAnimationVariableGreen->SetLowerBound(COLOR_MIN);
                if (SUCCEEDED(hr))
                {
                    hr = m_pAnimationVariableGreen->SetUpperBound(COLOR_MAX);
                    if (SUCCEEDED(hr))
                    {
                        hr = m_pAnimationManager->CreateAnimationVariable(
                            INITIAL_BLUE,
                            &m_pAnimationVariableBlue
                            );
                        if (SUCCEEDED(hr))
                        {
                            hr = m_pAnimationVariableBlue->SetLowerBound(COLOR_MIN);
                            if (SUCCEEDED(hr))
                            {
                                hr = m_pAnimationVariableBlue->SetUpperBound(COLOR_MAX);
                            }
                        }
                    }
                }
            }
        }
    }
}
```



Обратите внимание на следующие определения из файла MainWindow. h.


```
class CMainWindow
{

    ...

private:

    // Animated Variables

    IUIAnimationVariable *m_pAnimationVariableRed;
    IUIAnimationVariable *m_pAnimationVariableGreen;
    IUIAnimationVariable *m_pAnimationVariableBlue;

    ...

};
```



### <a name="animating-x-and-y-coordinates"></a>Анимация координат x и y

следующий пример кода взят из эскиза. cpp в [образце макета сетки](/windows/desktop/UIAnimation/grid-layout-sample)Windows анимации. см. метод Кмаинвиндов:: Креатеаниматионвариаблес. Для представления координат X и Y каждого объекта создаются две переменные анимации.


```C++
// Create the animation variables for the x and y coordinates

hr = m_pAnimationManager->CreateAnimationVariable(
    xInitial,
    &m_pAnimationVariableX
    );

if (SUCCEEDED(hr))
{
    hr = m_pAnimationManager->CreateAnimationVariable(
        yInitial,
        &m_pAnimationVariableY
        );

    ...

}
```



Обратите внимание на следующие определения из эскиза. h.


```
class CThumbnail
{
public:

    ...

    // X and Y Animation Variables

    IUIAnimationVariable *m_pAnimationVariableX;
    IUIAnimationVariable *m_pAnimationVariableY;

    ...

};
```



Переменные анимации — это числа с плавающей запятой, но их значения также можно получить как целые числа. По умолчанию каждое значение округляется до ближайшего целого числа, но можно переопределить режим округления, используемый для переменной. В следующем примере кода используется метод [**сетраундингмоде**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationvariable-setroundingmode) , чтобы указать, что значения должны округляться вниз.


```C++
hr = m_pAnimationVariableX->SetRoundingMode(
    UI_ANIMATION_ROUNDING_MODE_FLOOR
    );
if (SUCCEEDED(hr))
{
    hr = m_pAnimationVariableY->SetRoundingMode(
        UI_ANIMATION_ROUNDING_MODE_FLOOR
        );

    ...

}
```



## <a name="previous-step"></a>Предыдущий шаг

Перед началом этого шага необходимо выполнить действия [в статье Создание основных объектов анимации](adding-animation-to-an-application.md).

## <a name="next-step"></a>Следующий шаг

После выполнения этого шага следующий шаг: [Обновление диспетчера анимации и рисование кадров](introducing-windows-animation-manager.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Иуианиматионманажер:: Креатеаниматионвариабле**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationmanager-createanimationvariable)
</dt> <dt>

[**Иуианиматионвариабле:: Сетловербаунд**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationvariable-setlowerbound)
</dt> <dt>

[**Иуианиматионвариабле:: Сетраундингмоде**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationvariable-setroundingmode)
</dt> <dt>

[**Иуианиматионвариабле:: Сетуппербаунд**](/windows/desktop/api/UIAnimation/nf-uianimation-iuianimationvariable-setupperbound)
</dt> <dt>

[Windows Общие сведения об анимации](scenic-animation-api-overview.md)
</dt> </dl>

 

 