---
description: Параметры для Велдинг вершин.
ms.assetid: e73af63d-ed02-4fbc-8386-e8a40b0465ea
title: Перечисление D3DXWELDEPSILONSFLAGS (D3dx9mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- _D3DXWELDEPSILONSFLAGS
api_type:
- HeaderDef
api_location:
- d3dx9mesh.h
ms.openlocfilehash: c206718cd55a05d67d0a38d90c254238b63e964fa1f26149e75b57e09db359e4
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119044492"
---
# <a name="d3dxweldepsilonsflags-enumeration"></a>Перечисление D3DXWELDEPSILONSFLAGS

Параметры для Велдинг вершин.

## <a name="syntax"></a>Синтаксис


```C++
enum _D3DXWELDEPSILONSFLAGS {
  D3DXWELDEPSILONS_WELDALL              = 1, 
  D3DXWELDEPSILONS_WELDPARTIALMATCHES   = 2, 
  D3DXWELDEPSILONS_DONOTREMOVEVERTICES  = 4, 
  D3DXWELDEPSILONS_DONOTSPLIT           = 8 

};
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="D3DXWELDEPSILONS_WELDALL"></span><span id="d3dxweldepsilons_weldall"></span>**D3DXWELDEPSILONS \_ велдалл**
</dt> <dd>

Расшва все вершины, расположенные в одном месте. Использование этого флага позволяет избежать сравнения Эпсилон между компонентами вершины.

</dd> <dt>

<span id="D3DXWELDEPSILONS_WELDPARTIALMATCHES"></span><span id="d3dxweldepsilons_weldpartialmatches"></span>**D3DXWELDEPSILONS \_ велдпартиалматчес**
</dt> <dd>

Если данный компонент вершины находится в пределах Эпсилон, измените частично совпадающие вершины так, чтобы оба компонента совпадали. Если все компоненты равны, удалите один из вершин.

</dd> <dt>

<span id="D3DXWELDEPSILONS_DONOTREMOVEVERTICES"></span><span id="d3dxweldepsilons_donotremovevertices"></span>**D3DXWELDEPSILONS \_ донотремовевертицес**
</dt> <dd>

Указывает, что монтажный шов должен разрешать только изменения в вершинах и не удалять их. Этот флаг допустим, только если задан параметр D3DXWELDEPSILONS \_ велдпартиалматчес. Полезно изменить вершины, чтобы они были равны, но не разрешать удаление вершин.

</dd> <dt>

<span id="D3DXWELDEPSILONS_DONOTSPLIT"></span><span id="d3dxweldepsilons_donotsplit"></span>**D3DXWELDEPSILONS \_ донотсплит**
</dt> <dd>

Указывает, что расшов не следует разбивать вершины, наявляющиеся в отдельных группах атрибутов. Если метод [**ID3DXMesh:: optimize**](id3dxmesh--optimize.md) вызывается с \_ флагом D3DXMESHOPT аттрсорт, то \_ также будет установлен флаг D3DXMESHOPT донотсплит. Установка этого флага может замедлить обработку вершин программного обеспечения.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3dx9mesh. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Перечисления D3DX](dx9-graphics-reference-d3dx-enums.md)
</dt> <dt>

[**D3DXWeldVertices**](d3dxweldvertices.md)
</dt> </dl>

 

 




