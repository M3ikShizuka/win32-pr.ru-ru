---
title: Итссбтаржет Фармнаме, свойство
description: Возвращает или задает имя фермы, к которой присоединен этот целевой объект.
ms.assetid: 83e168ae-f985-40f9-912b-496c0695f82a
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства Фармнаме
- Службы удаленных рабочих столов свойства Фармнаме, интерфейс Итссбтаржет
- Службы удаленных рабочих столов интерфейса Итссбтаржет, свойство Фармнаме
- Службы удаленных рабочих столов свойства Фармнаме, интерфейс Итссбтаржетекс
- Службы удаленных рабочих столов интерфейса Итссбтаржетекс, свойство Фармнаме
topic_type:
- apiref
api_name:
- ITsSbTarget.FarmName
- ITsSbTarget.get_FarmName
- ITsSbTarget.put_FarmName
- ITsSbTargetEx.FarmName
- ITsSbTargetEx.get_FarmName
- ITsSbTargetEx.put_FarmName
api_location:
- Sbtsv.idl
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e5948656e356c7369d8aa28e4178ebb063c46a15
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122482380"
---
# <a name="itssbtargetfarmname-property"></a>Свойство Итссбтаржет:: Фармнаме

Возвращает или задает имя фермы, к которой присоединен этот целевой объект.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_FarmName(
  [in]          BSTR Val
);

HRESULT get_FarmName(
  [out, retval] BSTR *pVal
);
```



## <a name="property-value"></a>Значение свойства

Переменная **BSTR** , содержащая имя фермы.

## <a name="requirements"></a>Требования




| | | Минимальный поддерживаемый клиент<br /> | Нет поддерживаемых<br /> | | Минимальный поддерживаемый сервер<br /> | Windows Server 2012<br /> | | IDL<br /> | <dl><dt>Сбтсв. idl</dt></dl> | | IID<br /> | IID_ITsSbTarget определяется следующим образом:<ul><li>16616ECC-272D-411D-B324-126893033856</li><li>e85e10ea-db0b-4752-b456-5fd5840901c0 на сервере Windows 2008 R2</li></ul> | 




## <a name="see-also"></a>См. также

<dl> <dt>

[**итссбтаржетекс**](itssbtargetex.md)
</dt> <dt>

[**итссбтаржет**](/windows/desktop/api/sbtsv/nn-sbtsv-itssbtarget)
</dt> </dl>

 

 





