---
description: Создает экземпляр объекта Директксфиле. Не рекомендуется.
ms.assetid: c920d480-2557-491d-87ea-7eea1f470498
title: Функция Директксфилекреате (Дксфиле. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DirectXFileCreate
api_type:
- DllExport
api_location:
- d3dxof.dll
ms.openlocfilehash: 8ee1787941bbb902e6f0f50b082867aaf2f0a8bc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126964965"
---
# <a name="directxfilecreate-function"></a>Функция Директксфилекреате

Создает экземпляр объекта Директксфиле. Не рекомендуется.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT STDAPICALLTYPE DirectXFileCreate(
   LPDIRECTXFILE *lplpDirectXFile
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*лплпдиректксфиле* 
</dt> <dd>

Тип: **[ **лпдиректксфиле**](idirectxfile.md)\***

Адрес указателя на интерфейс [**идиректксфиле**](idirectxfile.md) , представляющий созданный объект директксфиле.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Если функция выполнена успешно, возвращается значение D3D \_ ОК. Если функция завершается ошибкой, возвращаемое значение может быть одним из следующих: ДКСФИЛИРР \_ бадаллок, дксфилирр \_ бадвалуе.

## <a name="remarks"></a>Комментарии

После использования этой функции используйте [**регистертемплатес**](idirectxfile--registertemplates.md) для регистрации шаблонов, [**креатинумобжект**](idirectxfile--createenumobject.md) для создания объекта перечислителя или [**креатесавеобжект**](idirectxfile--createsaveobject.md) для создания объекта Save.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Дксфиле. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3dxof. lib</dt> </dl> |
| DLL<br/>     | <dl> <dt>D3dxof.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Функции файла X](dx9-graphics-reference-x-file-functions.md)
</dt> <dt>

[**креатинумобжект**](idirectxfile--createenumobject.md)
</dt> <dt>

[**креатесавеобжект**](idirectxfile--createsaveobject.md)
</dt> <dt>

[**регистертемплатес**](idirectxfile--registertemplates.md)
</dt> </dl>

 

 




