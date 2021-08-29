---
description: Закрывает указанный куст автономного реестра и освобождает память, выделенную для Hive.
ms.assetid: e30a92dd-8533-406f-ad63-96306f125d78
title: Функция Орклосехиве (Оффрег. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ORCloseHive
api_type:
- DllExport
api_location:
- Offreg.dll
ms.openlocfilehash: 4852112ff1de3d0650c78b07a2ebbba780e89a485a176cf610fd2cf7b1fa234f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119824834"
---
# <a name="orclosehive-function"></a>Функция Орклосехиве

Закрывает указанный куст автономного реестра и освобождает память, выделенную для Hive.

## <a name="syntax"></a>Синтаксис


```C++
DWORD ORCloseHive(
  _In_ ORHKEY Handle
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Обработчик* \[ окне\]
</dt> <dd>

Маркер корневого ключа автономного куста реестра, который необходимо закрыть.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция завершается успешно, возвращается значение ошибки \_ Success.

Если функция завершается ошибкой, возвращаемое значение является ненулевым кодом ошибки, определенным в файле Winerror. h. [](/windows/win32/api/winbase/nf-winbase-formatmessage) \_ \_ \_ Для получения обобщенного описания ошибки можно использовать функцию FormatMessage с флагом формата Message от System.

## <a name="remarks"></a>Remarks

Функция **орклосехиве** освобождает всю память, выделенную автономными функциями реестра от имени указанного Hive.

Чтобы сохранить изменения в Hive, вызовите функцию [**орсавехиве**](orsavehive.md) перед вызовом **орклосехиве**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|---------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | Windows Библиотека автономных разделов реестра версии 1,0 или более поздней<br/>                      |
| Заголовок<br/>          | <dl> <dt>Оффрег. h</dt> </dl>   |
| DLL<br/>             | <dl> <dt>Offreg.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**оропенхиве**](oropenhive.md)
</dt> <dt>

[**орсавехиве**](orsavehive.md)
</dt> </dl>

 

 
