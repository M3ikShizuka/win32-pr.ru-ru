---
title: Класс CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION (D3dx12. h)
description: Вспомогательный класс для создания подобъекта состояния взаимосвязи ДКСИЛ-to-EXPORTS.
keywords:
- Класс CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION
topic_type:
- apiref
api_name:
- CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION
api_location:
- d3dx12.h
api_type:
- HeaderDef
ms.localizationpriority: low
ms.topic: reference
ms.date: 08/04/2021
ms.openlocfilehash: 84d8ae4ab76845d2e188d4be41e57b7770dfe89c
ms.sourcegitcommit: 0dec0044816af3f2b2e6403659e1cf11138c90cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "121813304"
---
# <a name="cd3dx12_dxil_subobject_to_exports_association-class"></a>Класс CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION

Вспомогательный класс для создания подобъекта состояния взаимосвязи ДКСИЛ-to-EXPORTS.

Дополнительные сведения о вспомогательных параметрах создания объектов состояния D3DX12 см. в разделе [CD3DX12_STATE_OBJECT_DESC](cd3dx12-state-object-desc.md).

## <a name="syntax"></a>Синтаксис

```cpp
class CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION
{
    CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION() noexcept;
    CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION(CD3DX12_STATE_OBJECT_DESC& ContainingStateObject);
    void SetSubobjectNameToAssociate(LPCWSTR SubobjectToAssociate);
    void AddExport(LPCWSTR Export);
    template<size_t N> void AddExports(LPCWSTR(&Exports)[N]);
    void AddExports(const LPCWSTR* Exports, UINT N);
    D3D12_STATE_SUBOBJECT_TYPE Type() const noexcept override;
    operator const D3D12_STATE_SUBOBJECT& () const noexcept;
    operator const D3D12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION& () const noexcept;
};
```

## <a name="members"></a>Члены

`CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION`

Конструктор по умолчанию. Создает новый экземпляр **CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION**, инициализированный по умолчанию.

`CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION(CD3DX12_STATE_OBJECT_DESC&)`

Конструктор, создающий новый экземпляр **CD3DX12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION** , инициализируемый с помощью содержимого объекта [**CD3DX12_STATE_OBJECT_DESC**](cd3dx12-state-object-desc.md) .

`SetSubobjectNameToAssociate(LPCWSTR)`

Для задания имени связываемого подобъекта.

`AddExport(LPCWSTR)`

Добавляет экспортируемый объект для связывания.

`AddExports(LPCWSTR(&)[N]);`

Добавляет массив экспортов для связывания. Параметр шаблона *N* указывает количество элементов в массиве.

`AddExports(const LPCWSTR*, UINT)`

Определяет массив *N* экспортов для связывания.

`Type`

Возвращает тип подобъекта, представленного [D3D12_STATE_SUBOBJECT_TYPE_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION](/windows/win32/api/d3d12/ne-d3d12-d3d12_state_subobject_type) константой.

`operator const D3D12_STATE_SUBOBJECT&`

Оператор преобразования, возвращающий ссылку на константу [D3D12_STATE_SUBOBJECT](/windows/win32/api/d3d12/ns-d3d12-d3d12_state_subobject) объект, описывающий объект состояния.

`operator const D3D12_SUBOBJECT_TO_EXPORTS_ASSOCIATION&`

Оператор преобразования, возвращающий ссылку на константу [D3D12_DXIL_SUBOBJECT_TO_EXPORTS_ASSOCIATION](/windows/win32/api/d3d12/ns-d3d12-d3d12_dxil_subobject_to_exports_association) объект, описывающий объект состояния.

## <a name="requirements"></a>Requirements (Требования)

| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок | [D3dx12. h](https://github.com/microsoft/DirectX-Headers/blob/main/include/directx/d3dx12.h) |

## <a name="see-also"></a>См. также

* [Вспомогательные структуры для Direct3D 12](helper-structures-for-d3d12.md)
* [CD3DX12_STATE_OBJECT_DESC](cd3dx12-state-object-desc.md)
