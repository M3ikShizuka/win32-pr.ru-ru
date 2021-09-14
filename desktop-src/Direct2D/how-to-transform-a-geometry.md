---
title: Преобразование геометрии
description: Показывает, как преобразовать геометрию с помощью Direct2D.
ms.assetid: de434615-14b1-4b66-b09b-e90468e03d58
ms.topic: article
ms.date: 05/31/2018
ms.custom: seodec18
ms.openlocfilehash: ae15d0b1da304f9dfe24ff5de33a9f1582e2ca05
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163135"
---
# <a name="how-to-transform-a-geometry"></a>Преобразование геометрии

Чтобы преобразовать геометрию, можно либо применить преобразование к целевому объекту отрисовки, вызвав [**сеттрансформ**](id2d1rendertarget-settransform.md) , либо применить преобразование к геометрии, вызвав [**креатетрансформеджеометри**](/windows/desktop/api/d2d1/nf-d2d1-id2d1factory-createtransformedgeometry(id2d1geometry_constd2d1_matrix_3x2_f__id2d1transformedgeometry)). Хотя оба подхода преобразуют геометрию, они имеют некоторые фундаментальные различия. **Креатетрансформеджеометри** влияет на заливку, но не влияет на ширину штриха. Кроме того, **креатетрансформеджеометри** преобразует только геометрию, не затрагивая другие фигуры в целевом объекте прорисовки, тогда как [**сеттрансформ**](/windows/win32/api/d2d1/nf-d2d1-id2d1brush-settransform(constd2d1_matrix_3x2_f_)) применяет преобразование ко всем фигурам в целевом объекте прорисовки.

В этом разделе приведены инструкции по преобразованию геометрии путем вызова [**креатетрансформеджеометри**](/windows/win32/api/d2d1/nf-d2d1-id2d1factory-createtransformedgeometry(id2d1geometry_constd2d1_matrix_3x2_f__id2d1transformedgeometry)).

**Преобразование геометрии**

1.  Объявите переменную [**ID2D1TransformedGeometry**](/windows/win32/api/d2d1/nn-d2d1-id2d1transformedgeometry) .
2.  Вызовите метод [**креатетрансформеджеометри**](/windows/win32/api/d2d1/nf-d2d1-id2d1factory-createtransformedgeometry(id2d1geometry_constd2d1_matrix_3x2_f__id2d1transformedgeometry)) , чтобы создать преобразованную геометрию.

В следующем коде показано, как создать почасовое стекло, преобразовать почасовое стекло и нарисовать исходный и результирующий очков.


```C++
// Create a path geometry.
if (SUCCEEDED(hr))
{
    hr = m_pD2DFactory->CreatePathGeometry(&m_pPathGeometry);

    if (SUCCEEDED(hr))
    {
        // Write to the path geometry using the geometry sink.
        hr = m_pPathGeometry->Open(&pSink);

        if (SUCCEEDED(hr))
        {
            pSink->BeginFigure(
                D2D1::Point2F(0, 0),
                D2D1_FIGURE_BEGIN_FILLED
                );

            pSink->AddLine(D2D1::Point2F(200, 0));

            pSink->AddBezier(
                D2D1::BezierSegment(
                    D2D1::Point2F(150, 50),
                    D2D1::Point2F(150, 150),
                    D2D1::Point2F(200, 200))
                );

            pSink->AddLine(D2D1::Point2F(0, 200));

            pSink->AddBezier(
                D2D1::BezierSegment(
                    D2D1::Point2F(50, 150),
                    D2D1::Point2F(50, 50),
                    D2D1::Point2F(0, 0))
                );

            pSink->EndFigure(D2D1_FIGURE_END_CLOSED);

            hr = pSink->Close();
        }
        SafeRelease(&pSink);
    }
}

if (SUCCEEDED(hr))
{
    // Create a transformed geometry which is tilted at an angle to the previous geometry
    hr = m_pD2DFactory->CreateTransformedGeometry(
        m_pPathGeometry,
        D2D1::Matrix3x2F::Rotation(
            45.f,
            D2D1::Point2F(100, 100)),
        &m_pTransformedGeometry
        );
}
```



 

 