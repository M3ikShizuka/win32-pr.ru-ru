---
description: Структура D3DXMATRIX (D3DX10Math. h) — матрица 4x4, содержащая методы и перегрузки операторов.
ms.assetid: c354d28b-bb08-41c5-bb59-90a912181f0f
title: Структура D3DXMATRIX (D3DX10Math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXMATRIX
api_type:
- HeaderDef
api_location:
- D3DX10Math.h
ms.openlocfilehash: 0d2489031254dc3d97fd65690de208c0fa9fd37a3bdb2b039a6a8f076092edb6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120070174"
---
# <a name="d3dxmatrix-structure-d3dx10mathh"></a>Структура D3DXMATRIX (D3DX10Math. h)

Матрица 4x4, содержащая методы и перегрузки операторов.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct D3DXMATRIX {
  FLOAT _ij;
} D3DXMATRIX, *LPD3DXMATRIX;
```



## <a name="members"></a>Члены

<dl> <dt>

**\_иж**
</dt> <dd>

Тип: **[ **float**](../winprog/windows-data-types.md)**

</dd> <dd>

Компонент (i, j) матрицы, где i — это номер строки, а j — номер столбца. Например, \_ 34 означает то же, что и \[ ₃ ₄ \] , компонент в третьей строке и четвертом столбце.

</dd> </dl>

## <a name="remarks"></a>Remarks

Программисты C не могут использовать структуру D3DXMATRIX, они должны использовать структуру D3DMATRIX. Программисты C++ могут воспользоваться преимуществами перегруженных конструкторов и операторов присваивания, унарных и бинарных (включая равенство).

В D3DX \_ элемент 34 матрицы проекции не может быть отрицательным числом. Если приложению нужно использовать отрицательное значение в этом расположении, необходимо масштабировать всю матрицу проекции на-1.

### <a name="d3dxmatrix-extensions"></a>Расширения D3DXMATRIX

**D3DXMATRIX** имеет следующие расширения C++.


```
#ifdef __cplusplus
typedef struct D3DXMATRIX : public D3DMATRIX
{
public:
    D3DXMATRIX() {};
    D3DXMATRIX( CONST FLOAT * );
    D3DXMATRIX( CONST D3DMATRIX& );
    D3DXMATRIX( CONST D3DXFLOAT16 * );
    D3DXMATRIX( FLOAT _11, FLOAT _12, FLOAT _13, FLOAT _14,
                FLOAT _21, FLOAT _22, FLOAT _23, FLOAT _24,
                FLOAT _31, FLOAT _32, FLOAT _33, FLOAT _34,
                FLOAT _41, FLOAT _42, FLOAT _43, FLOAT _44 );


    // access grants
    FLOAT& operator () ( UINT Row, UINT Col );
    FLOAT  operator () ( UINT Row, UINT Col ) const;

    // casting operators
    operator FLOAT* ();
    operator CONST FLOAT* () const;

    // assignment operators
    D3DXMATRIX& operator *= ( CONST D3DXMATRIX& );
    D3DXMATRIX& operator += ( CONST D3DXMATRIX& );
    D3DXMATRIX& operator -= ( CONST D3DXMATRIX& );
    D3DXMATRIX& operator *= ( FLOAT );
    D3DXMATRIX& operator /= ( FLOAT );

    // unary operators
    D3DXMATRIX operator + () const;
    D3DXMATRIX operator - () const;

    // binary operators
    D3DXMATRIX operator * ( CONST D3DXMATRIX& ) const;
    D3DXMATRIX operator + ( CONST D3DXMATRIX& ) const;
    D3DXMATRIX operator - ( CONST D3DXMATRIX& ) const;
    D3DXMATRIX operator * ( FLOAT ) const;
    D3DXMATRIX operator / ( FLOAT ) const;

    friend D3DXMATRIX operator * ( FLOAT, CONST D3DXMATRIX& );

    BOOL operator == ( CONST D3DXMATRIX& ) const;
    BOOL operator != ( CONST D3DXMATRIX& ) const;

} D3DXMATRIX, *LPD3DXMATRIX;

#else //!__cplusplus
typedef struct _D3DMATRIX D3DXMATRIX, *LPD3DXMATRIX;
#endif //!__cplusplus
        
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3DX10Math. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Структуры D3DX](d3d10-graphics-reference-d3dx10-structures.md)
</dt> </dl>

 

 
